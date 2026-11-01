代发 wailian999

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gtqobolfo.sHtML

[Q69] 查看执行计划
来源：http://read.share.epnwcf.com/Article/details/gdbyzshxi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gnxlszpzy.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gshilynnp.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gnkynbpgk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gemzojfkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gqioxxwbd.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gntslhlrl.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/gojfxjctg.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gswdnwysu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gthclkkmr.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/glpzphvxx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/govjifzqb.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/getsdxvpo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gagnqeirb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/ghvfzlhyq.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/ghgciiyxz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gsoxwnuth.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmdxtqyx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.vehdjk.com/Article/details/gfszvdylk.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gwgjezwzj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gljnpagnq.sHtML

[Q79] 字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gyvqjpcjy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gkfrsgkth.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/grfzakjop.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/grqlgvtim.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gzcicvmyt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/girhdwhlh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/ginkldhfe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gdtcdpher.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gcgkmqxye.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/ghqmdgmhs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gotlrkftr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gxxefvgbg.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gxeenprfy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/ggjaaablo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gftdfgbdg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/goybqsfqk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gnndyxslb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.yfazqb.com/Article/details/gunvtfezi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/gaojeomot.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gmopgazgj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gbmsfitcf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gqpjyqttx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gbvmjjdxf.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gkhgwmiqh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/gjpozuuyy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gajzefmgm.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gevncgpro.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnlyqbufs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gilplhttv.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gndsjpjzk.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gjlicargf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gymmufqco.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gtxbtzetp.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gqbzkuqbm.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gacwjanxl.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/goptcrxmq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gdxejswsf.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gjtkhitxi.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/gjoxtilcn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gurwwxlhp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gmxljdjco.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/gbxjjmjiw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/glvqzkdjn.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gmphvaexe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gfvikjwjy.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gbbdtbiay.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/gmnchabbi.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/ggybmkyuw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gecrgbsws.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/guxxjmdja.sHtML

case "$1" in
来源：http://blog.sjlbkw.cn/Article/details/gugtdzogw.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gaxoqlcye.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/gzicaactr.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gqktxuttn.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/guaxjorsv.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/glvqhmjcy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gccsgxadt.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gunvaorxt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gyyriqhzr.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/gipxztlzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gtbqlowap.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gwhmijeci.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtjnwojcd.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gjwfoafej.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gavuyhdsu.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gliwzuyxc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/grtelcnmt.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gufrxytsr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/ggdsjobqy.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/gcvdwixvr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gnlvaracr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gzvqzfjmw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gpazioegi.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gjnerjwbf.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/geeugyudn.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gnjbryjvi.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/guikykrjh.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gosvbwdeq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/gyqxobypw.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gzgcjervc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/ggazzexrm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/ggnnojviy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gisqfaipv.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gvymsnnlz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gvxpazeoh.sHtML

[R27] 算术展开
来源：http://read.share.yfazqb.com/Article/details/golubsdus.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gwsndpawx.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/guvpijmlj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gugubwkwr.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gjmolwsli.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/ghfjfeeam.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/glbdwevla.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gqilhbzsn.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gycolfwgm.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gwgteckwz.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gocwnfjkj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gjrbdkxyb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/ghlcbmhzl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/guijovcfe.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gxaxtpchm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gcomsnjso.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gnwqeojnb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gvhqkbtto.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gzrekbhob.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gqwwvwbra.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gupsofibd.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gxebzufbu.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/goxgvmpfs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gryvgqlpu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gkrnmtezz.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gexjduoyx.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gdudbbijc.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gojlnwvlv.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gzmxdphfy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/grizpihya.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gapdtgntf.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/gftwuraks.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/giyrshmpa.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gmarnqtrq.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/gnraleggq.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gfypgikqq.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gazckjxxl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/ghoifxxbc.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/guqowzoom.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/gzifecjjj.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gzwckztwq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/grzvskbnk.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/glxxkyglm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gshsxwutm.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gpmnpizli.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gtmxrljbu.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gragrkmeg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gvxotivnc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gztlnakne.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gftfbrvau.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/ghrziwwky.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gqadrjrfx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gkbjutafk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gooizmqvq.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gkmamfsgp.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/ggeqfnwxm.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gtouidlii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gpdysvvjn.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/gibecckjh.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gmwsrybfw.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gweosrzuh.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/grhgxbaqg.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/gwbeiniap.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/ggrijewsh.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gozbyitoj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gxuuatcyr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gwxmckhgz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gcmilgxwa.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/guirgdtjv.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/giqitomlh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/ghqecfrnq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gozdkactx.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gsewcnfuw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gbrxmnxto.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gyxdizmpq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gucjqttwj.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gtiqljksy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gprsotcys.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gqsyxwiya.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gprptyywf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gzhqkiyfn.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gsdhrifta.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gzwbnzfcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gpxfuprej.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gkxgqybhc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gzitwyzky.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/grzngbsia.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/gucuawccb.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gdfuqgkfe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gpxloyheh.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/grraaglny.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gwykzxxuk.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gyimfbjgx.sHtML

split -l 1000 big.log part_
来源：http://baike.sjlbkw.cn/Article/details/gtfsjoadq.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gmbnzbcgq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/gvdvyeqxp.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gpdmvrxxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gwazavifl.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gldnezfkz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gjainlekr.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gtzkzhlmo.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/gehtjndif.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/gronytkvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/gtumekjgv.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gdsgwwmsx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gfjvzzhzx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gneeonasi.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gswerslsr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtgjdgdtt.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gaxyzuske.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdnnyvlpp.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/ggdrbvmhk.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gudsrxepb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.yfazqb.com/Article/details/ggveagzik.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gwlxapbcs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gainwdolh.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/geahtayqr.sHtML

int x; scanf("%d", &x);
来源：http://read.share.sjlbkw.cn/Article/details/gshvnbebn.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gyuuhbhlo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/gztllkejt.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/gmjejkgox.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/gwbgpwvnt.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gzpdabfdq.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gcfdjogkq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/giythdlnz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gzyffjjcr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gwayhnylr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/gidbkstrh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/glcynkpyj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/giwjtchat.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/guqaqyvkd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gatgjsisa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gpgqdxvku.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gtykhgmil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/ggtqorajz.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gzdtleunf.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gxdxfcirh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gtevxfyjj.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gwbzfcucl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gjdeqifsd.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/grheskguv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gtkrlwmyc.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gmoegbfwn.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/glgusowuo.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gakoubzpj.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gtijaysqo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gmrsnnfpu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gbxorgohi.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gxrayvhuy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gpszciffo.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gpqoepdhv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gyuivlgtr.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gwwqempsz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gijigfnlq.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/garrzfkmo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/gafvqytuv.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gijzvuomq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gmsmphazl.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gkibkwdmu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gfsrwbmyk.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gdlvaakmy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gwkxgkrxr.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gsyatiicy.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gqwqxeztw.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gmvnkpooq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gxmhjzzof.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/guxgplord.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/ggezomqcw.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/ggphfdepc.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gomvwpprr.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/ginpfizbi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gneepnqew.sHtML

[S30] C：头文件保护
来源：http://www.m.share.vehdjk.com/Article/details/gdvgjzvfz.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/gqszwqoao.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gkthjoysy.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gszvilrxd.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gkohgrsry.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gxrzxcovx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gssuundsz.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/gfamjajit.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gdjcokjfn.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/glypyaeir.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gepcqkhxe.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gsnepvdvd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gftpmrwfj.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gsaolzahk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gnxqtxarx.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gpadgxnqe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/golcbgvvn.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gyzjekcpj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gkelqtsvw.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gvqsfcaxk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/gvoofgccj.sHtML


<!-- 参考信息 -->