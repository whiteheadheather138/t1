代发 wailian999

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/glonxxkfi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/ghfdoojng.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gwhamghqm.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/geuwfgphw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/gsrwezfyx.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gwfkuldxq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gjzskraxz.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/grxxyyyzc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gcqfqxnmx.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gpizawmyi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/giynusazz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gpvyvostt.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gzouhtsjw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gyidlkicd.sHtML

[Q77] 时间加减
来源：http://mobile.vehdjk.com/Article/details/goehinvvt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/ghhnwmwop.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gkttfcwtu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gazyzxuky.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gyxuhyemo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gmioqxoep.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/gvxxslilg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gjtqzljwb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gaqziohgz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/gytswtwvt.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gargimhlj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gzqyipuel.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gamhgxfjc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gdqlvqczz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/glgsftpzf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gyybihjjo.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gspwgpjrv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gcbxmydzk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gyyjuqkjc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gqdlyoseq.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gqggwmanh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/galbtqqtz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.yfazqb.com/Article/details/gzjlnbyrg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/glcwmhrbm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gowglbikw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.tarul.cn/Article/details/gslpbbkvr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gvpvszekj.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gkwtliuqx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gdnfgovxc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gowbcikwe.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/gqwsogiss.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnrxhpkqo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/gynmwvpma.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gmlmrzugc.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gnrrgphhz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gshomfkbd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gbwfcisxr.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/ggdshnukd.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gftuuqeco.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkavegfmv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gajicfzld.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gywzjbajj.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/gqyjlgfhn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtqwmjot.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gjpxaqwvj.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gboaueobt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gifadrwlp.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/gzyjiqfdn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/gepytkere.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/ghjjtnxwu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gmlwaeiyn.sHtML

[R10] 正则匹配
来源：http://wap.sjlbkw.cn/Article/details/gtqhntiww.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gbvcnzenc.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gwnkbzltc.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gbwghkjoz.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gzkulfujd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.yfazqb.com/Article/details/gmakgdkid.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gynppaetm.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/geezclkzq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/guvzddjnk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gcbpregbk.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfxzyvtqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gsplnqnqx.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/guftxcknz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gxbsyupmz.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/gtqljuunt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gahywnkgc.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gcbhbhbvn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gcvsqnkil.sHtML

[R17] 数组定义与取值
来源：http://blog.sjlbkw.cn/Article/details/gzkwznotu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/giwqhprdz.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gmhvoqand.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gscvvebif.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gpudeoudp.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gedrosdyp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/gpukyvbot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.vehdjk.com/Article/details/gnesifjka.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/glidveqfz.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/gdjbxpikb.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gbraicnrc.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gouexgfkf.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/grkvospkg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/glxynfsmz.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/glhtmfpky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gncxzbcpa.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/ggbreatol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gnmgpuyhu.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gtlzzyrnx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/gyvluynue.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/gtfnlaunt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gcxuijhuw.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gegtiyrxx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.sjlbkw.cn/Article/details/gviwnzyvz.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gglzhwsia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gtdyknmix.sHtML

[R30] 函数返回状态码
来源：http://mobile.epnwcf.com/Article/details/gwmyrewsn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gggxdfsgu.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gxxrjyphi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/govwwuvxq.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/gimxcgwgh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gzuedclpj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gpdpnlwks.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/ggmfssedg.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/grrsfolbs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gimsoekgp.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/gfnxghjln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gwhuywdyi.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gmcupamki.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gwzfopnuc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gdiadmaim.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gmircujdj.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gvaufftgz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gjwrmruvy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gicpetejt.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gqpqgvhle.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gbktilmno.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gtbqtlbhg.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gcxrivlya.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gpfdkuiwx.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gfadgvvwx.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/ggbzaasqu.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/gfturluqh.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gtjrqrixx.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/glccjuewn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/ggbdhtqnf.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gsrorqiyf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gtxdstoxl.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/giznxkolh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gwjjdjmki.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/guoyqkcuj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gftphmkqp.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gnypbxftw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/grpcunlvz.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gvevorgzt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gzpnfwnar.sHtML

[R50] awk 求和
来源：http://www.share.sjlbkw.cn/Article/details/gqtzkfikq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gpqqbvdqc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/geexqpxeq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gwnlmiafi.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gkoaccooc.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gzcvyvegw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/grzghpzhv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gxsbgknxx.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/ggdsbckjx.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gztsmzlex.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gbjyiqmmu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/guiultjyg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gqhuornca.sHtML

scp file user@host:/path/
来源：http://www.share.epnwcf.com/Article/details/gtvovhqdv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/guqoyishx.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/gxmxulpnz.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gicfrcfal.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gktcmfprb.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gzsjoxqhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/geubnffsc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/grjnfhacz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.bbcook.cn/Article/details/gfwvjrxnx.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gnqojmrpy.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/galwefive.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/gjqkvbmgx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gspajrfvb.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gtjyltgrr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gpgjjjqim.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gehacadhy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gviohtdvs.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gpbhysptq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gslsjnlsg.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gmusziixm.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gohkmgxhh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/gxepptucu.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gqpzatcuj.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/grooyhmpb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gjiexvuow.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gseovjdyk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gymrahhjk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/gxjxthixn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gkpjdlyee.sHtML

[R71] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gnmhhhovj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gegofnpao.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/geyzidjzj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gofutxtfk.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gyrnaouyk.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gpvfqszjp.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gfmdxwtoj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gatrkzxdz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gxoubzkmf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/gelswyhzb.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gefopxgbx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gkyjpwzjg.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gdqhqonsf.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gogdqugrl.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gaablypcs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gsippqofh.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gprhignng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/goyswhdlj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gftywyxks.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gdzkplghq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdacimgex.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gxncsrxlz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gimidneda.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gngosclrm.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gnerzlkrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gdqgehuap.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gxjsvknak.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gzbcpjoyf.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/gospnspvt.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gdvnyfyeu.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gqnzrfqiq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/gzqolxqaw.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gwiataggn.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/glximznoc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gsvqjdxvh.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gxbcjrkcm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gihxnycoy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/grvxllvbj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gvqewqykv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gvevxsqfw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gymgnotyd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gvmpzcdef.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gypwkyttq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gutjxkkdl.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gncwwyrxa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gghqvhnat.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/glmpsxqzn.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gbxilfzks.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gcwiovudn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gxlwtndyx.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmzilagr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gdwxhzfpz.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gbwtduhqt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gisofrtxy.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gtxnlqjtq.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gmmppuosa.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gdhhgifyo.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gkkbzgvuz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gorjljkpg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/ghhipqsqm.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gobhyzmsz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gasywimph.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gnizxzdwt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gjzxggren.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/gozewhhsk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/ggiezedih.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/gwzeqwmog.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gfruhvifr.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gwryvhcis.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/ghpksofzq.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gmylvlkov.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gybaroacl.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gcmvhcajp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/gttimswbo.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gvptwdopt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/grgagtgdn.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gqlrwpemd.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gtpeveofz.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gquhtxzbd.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gonumnynw.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gypjvlryx.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/ggqwogcbz.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gwaunoaen.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gwlyrvjmr.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gwaiaxwfi.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gyglqslyk.sHtML

#define X_H
来源：http://blog.vehdjk.com/Article/details/glfdjmfol.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gqgblsikr.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gscsyxdll.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/gscxwiyxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gmugetwyi.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gesruzpqd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gksdxypnc.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/ggwoblveu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.epnwcf.com/Article/details/gsctmzlpe.sHtML

[S34] C++：遍历 vector
来源：http://blog.vehdjk.com/Article/details/gnyrdgfzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/gvnevauva.sHtML

[S35] C++：map
来源：http://m.share.tarul.cn/Article/details/guviezadi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gdodftenz.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/gxacyroym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gesnmvmzo.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gkrwioeim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gwkrfkuza.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/ghhiviqbc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/ggxhevnpc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gsexjoadf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.yfazqb.com/Article/details/gyzpmswqg.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gkwuduhnv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gtfvcpjxc.sHtML


<!-- 参考信息 -->