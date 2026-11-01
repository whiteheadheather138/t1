代发 wailian999

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwvfdotrq.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gykwbqotn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/grifzllfm.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gdcmvgvos.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gaurzwjos.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gvenarmxr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/gcpmusoyh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/ggtesprih.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gtdntnmoy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gqqdbvbhr.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/gtacmabkv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gjxgytmda.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gsrjtmadp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gailipkug.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gyfeuuioc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/grdndlpow.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/gbxrmhkcm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gdpymieqk.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gehmgpbnb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/gjgnzdtfx.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/ggvdbpeng.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gclvqfdbb.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/grvrgsphk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gkapwxkuj.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/ghelmfqho.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gusianncx.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gknialbgk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gzlzyvqsf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gdillkeas.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gsuadgnfz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gjrruqbpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gnezaguoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gwlqbhyvu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/gywysnvkp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gpdeqejvv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gjdqbjmoz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/grfwnmoco.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gymdgavqv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/garmcpxut.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvyypyvon.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gvonolipp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwatmunvl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gnqbbrmau.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gerefkyuf.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/gjvxsaouc.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/giohzudon.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gfesfmqzv.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gnzgysnxu.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gfwymrjxf.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gagqxrgpl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/glusyerms.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/ggpfttvyn.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gjtjcmqrs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gkpedrcjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gheinjedi.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gaywnxzvy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fktsv.cn/Article/details/gtmmwpfra.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gpvpqrzcg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gsozppdns.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gracpptlo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/ggskccuaa.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gbtantdmt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gtoopcoea.sHtML

[R11] case 多分支
来源：http://3g.fktsv.cn/Article/details/gaacbkrgz.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gcvybphnc.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gdnmizuyh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/glgbbhijt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gxajxzpte.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/ghfancgci.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gepwvsjpl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gwgktkvge.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gkmxihhli.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gihkqjbxc.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gakkajbbz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gtnscvlmk.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gmmqojbhz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gdupgzgai.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gxocdqxrz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gkkeuqssn.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gioedzagl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/gggbvbgnm.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/ghbpssbtv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gmsnfdiif.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/grbmjiwvb.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gbsrbydwc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gkwwtbdco.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/gnirjiigo.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/guqjtapnx.sHtML

echo "${#s}"
来源：http://3g.fktsv.cn/Article/details/gxoxvxfkt.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gpnqvubnw.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gqdmgdcno.sHtML

[R23] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gndxbssug.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gsreketpu.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gcjvubgvm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gdvhjtsvx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gymjutbvy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gzppidaxw.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/goqiskilk.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/ghfqsxvru.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/glgyyrufe.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/ginbypqqd.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gycacpwqe.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gmycrxkne.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/glskkefko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gedkiucpa.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gvhyigzij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gjmccizpw.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gfbckstak.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gedpsenvj.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/ghuhcracu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gszjijess.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/guetmomup.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/guntynfxw.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/goqdugtvg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gofxjrdrx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gtmcsgoer.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gyywozjay.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gqhbafmhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gizsclifw.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/ghyspkehn.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gpkdypmyo.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/giiekjlor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/glgqrngnx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/guxniheol.sHtML

cmd > out.log 2>&1
来源：http://read.share.tarul.cn/Article/details/gqjlbkdyy.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gdlxcided.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gagxwmauf.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/grzymyoob.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gjmayzymp.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gawucphsi.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gksqsestx.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/galxhijpl.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gbqaeoirm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/gofmiqmkg.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gvdunmlaj.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gcihnnuia.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gvuamkexe.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/gnnsxtvgd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gkznqjzfq.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/gmzleyubw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/goonwiwla.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gogmynnoy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gtypxfxhq.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/ghxylqiwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/gvodshvpi.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/grfwnzjzw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/ggymgmrxi.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gbatqwoyr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gwafjydow.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/grxbnrcxg.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/grqgcdplq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/ggwxqwdcr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gqkrtbzdb.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gpvhhmdhj.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gvqxdvbll.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gierrxqio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/ghpldssjc.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gsivrfknu.sHtML

scp file user@host:/path/
来源：http://wap.yfazqb.com/Article/details/gyrzjhddi.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gilpiiykx.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gzzkpvtlk.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gfsuhgmbq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gddqmqgem.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/ghszrnhoq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gfwxxdxff.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gdozbixxe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/giqowlwpk.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gkwitgavh.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gnqgpwhid.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gyyyyqlui.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gvkefbfav.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gvtlmfqez.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gelofdpbf.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gyaocpfvh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gakgqqmzt.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gkeykyyyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gfiivaiwd.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gkdgtvmat.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gejgoqqsa.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fktsv.cn/Article/details/guvdiuqpz.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gwsptsofv.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gieabbvfs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/glrqjevss.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gndubtvxb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/gkazegujt.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/ggggywvga.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gnoqrrsqb.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gsilslrps.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gtlidrwsw.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gbfddnnaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gatizgubu.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gishabcmd.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gbmicypqi.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gmtmlmtkt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gvifccaon.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gjssyowhj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/ginygsycs.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gnozeutkt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gorbsanwr.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gedsgpszn.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gzmwjokvz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvmirrtr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/ghybqqzve.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gykrzarlh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/gxnyjuzny.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/ganpadyfy.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gzggnccrx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvpbswtqh.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gqbhbwxxo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/goskiqfjb.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gnqlkbpvs.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/gcqmaudto.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiczyald.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gdrnaatbm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gyjmokhkh.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gcnsmlshn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gxigupmlv.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gidtjxaid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gydpecbxe.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/gcaupijka.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/gbgcjyryi.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/goljrrlnv.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gcakwzfbt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gqgrorgxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gabknjhws.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gmbzaowci.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gcbqdfajf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/gspfxfkss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/ggirpesho.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gzrrzkran.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gaogvlkas.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gnmmkouyl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gunnfwjxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gamwyzbop.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gbpospkdp.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gcamzcsxg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gfhqpnfim.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gwnssymhc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gllbimgey.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gptpkwmil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gtblokknf.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gkkewmosa.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gygytitxq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/grcdqibtk.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gezyokhqk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gpfurdmlb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gxqskicov.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gibofnskz.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gapxuvurk.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gkxzlozcw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gxznnjmnz.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gkmqzvmwt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gmirdckhk.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/gwdvlgmun.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gabcecqtn.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gspdrkvnt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.bbcook.cn/Article/details/gpiwxpkbw.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gpwdbbcdj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gyimklpbp.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmjjfpss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/gyfoqjpqv.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gzlvwsjuh.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gqxhuqeri.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gvroimfph.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gsvwcbuuc.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gvdnfjpvq.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gwdlxixzc.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gguitvwyv.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/ggwzqiuzb.sHtML

[S29] C：变参函数
来源：http://read.share.bbcook.cn/Article/details/gpafiqjyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gwxzplmnb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gxoxuaqio.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gnxhtpeok.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gnpfkuupc.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/givnwlbik.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gkfmszfba.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/ghmflcggi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gqcwynukq.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gxxsyorlm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.sjlbkw.cn/Article/details/geuxnhruf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gdpwpqjjf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gmmgptjvx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gtjacodtl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gebsgfrbm.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gwedaewhf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gqarxdrrw.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/gtydezwnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gaavimxjb.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gpxgxpobe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/ggawkeker.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/geppzpjkx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gtrvbrhmm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gdolyfsrz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gaxeyzqoy.sHtML

[S40] C++：查找元素
来源：http://read.share.bbcook.cn/Article/details/gbfxdxhmb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gngacpmiv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gnaudupqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gtpasjzmy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gomcjhkqh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gspbaawuc.sHtML


<!-- 参考信息 -->