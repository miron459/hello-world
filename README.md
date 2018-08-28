# hello-world
just
%%----------------------------------------------------%%
clear all 
%%
c='1.bmp';
L=imread(c);
s=size(L);
%%
%for i= 1 : 1 : 256 
%    qw=find(L==i-1); % подсчет распределения 
%    g(i)=length(qw'); % перепись n(i)
%end
%t=0:1:255;
%%
%plot(t,g); % график распределения вероятности
%hold on;
for i= 1:1:s(1)
    for j=1:1:s(2)
        if L(i,j)<15
            L(i,j)=255;
        end
    end
end
imshow(L)

