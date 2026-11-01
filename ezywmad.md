代发 wailian999

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gokkssrxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gifaqmofa.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/gfsgbcjwt.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gcknrcsxn.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/gxfxxuuat.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gjftzesek.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/geklaevic.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gullzibym.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/glwjxibcx.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/giemlntbd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gqfzsljkt.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/giguaneap.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/gavketytz.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gvahhzjrq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.bbcook.cn/Article/details/gybqgkndb.sHtML

[Q74] 强制使用索引
来源：http://blog.sjlbkw.cn/Article/details/gqwpuymqr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gqutzsktr.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gdlgrwchq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzorsbcie.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/gevaosmaf.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gyvgneciu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/ghvaeqxgr.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gtbszgjoq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gyjddilvn.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gersnfjxo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/grpobnipu.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gbmepiepj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/ghuprrmnw.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gqrkrvysf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gpwgmssco.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gfclleyfv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gusdefdkv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gcxwjunfx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gwqecfezy.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/glbtcimit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glvpfwxqg.sHtML

[Q84] 去除首尾空格
来源：http://blog.epnwcf.com/Article/details/gfyppcbcc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gkscdfoyq.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/guemtwjqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gmplhbkxz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gjwwmchag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/gbcesycuv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gqgeiyfch.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gczmmprth.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gfqyltdgn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/gfcjxwwmw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxnbpdyzw.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gmvvwkixl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gszfhtcne.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/gdcdsmbwy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gddlikhan.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqaiwqstr.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gvohoexyv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqxzyfdxi.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/ggxhruzru.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gvllqxksy.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gmfhrscgh.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gzczworee.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/ggcntqskr.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/gihwuvegg.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/giwgguzwz.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gpskvozfw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.epnwcf.com/Article/details/gzivbazeq.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/giinbmpna.sHtML

name="${1:-default}"
来源：http://wap.vehdjk.com/Article/details/gmsskxtse.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gbxbkzxzv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gtoukjoti.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gaboxhmlp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gcesnswdp.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gnxbzlsff.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gebudlgwn.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gwpsmhinx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gcduyvzcc.sHtML

[R10] 正则匹配
来源：http://wap.epnwcf.com/Article/details/gqlpnbaod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/geqhgjghy.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gejrflvqq.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gmyaijftu.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gudedpsda.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/gondjxxvk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gatpfmtzv.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gshddaigy.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/ghymybksf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gwjhqzoex.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gjqzkopcj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gxugwihql.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gleszfzxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gjiuycksf.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gkieryggg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gjllshsjw.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gvspyjmzk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gmwliuxob.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gctkhoqou.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gubuuitpf.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gfkikzapy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/glydjlcrz.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gzpxbnfph.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gbesuqgyz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gecgtrdun.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/ggwsjvuqw.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/ghskqfemo.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gfbhzzbgy.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gemyszckf.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gefrupozq.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gbalmzgcl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gwoyudhbl.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gfafhassk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/gzjztsoly.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/gyiumwgvn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.yfazqb.com/Article/details/gjoksyqad.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gxhhpatzb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gxqgiknjq.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/gnkgrecaa.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/grjzxyeho.sHtML

[R28] 浮点运算
来源：http://www.share.fktsv.cn/Article/details/ggeieilaq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gwhfftevy.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/giqipglii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/guqzxnwhb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gzymxlgry.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/grhtlkaob.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gszbzygeq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gmttgvgoe.sHtML

[R32] 参数个数校验
来源：http://blog.sjlbkw.cn/Article/details/gcynfjxdo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gtukormpr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gsnahwdvg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/givmqyufd.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gmdszihby.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/ggahbvygy.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gmtfwpzjm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/ghiahyzux.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gxjwevqjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gjcqeabbl.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gthkhjecw.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/gccyfatdc.sHtML

[R38] 管道串联
来源：http://www.blog.vehdjk.com/Article/details/grsbcliys.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/giqdonutq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/gfvhnkplh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/geqlqdhph.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gdaqzlimu.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gfsbgfoxf.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gyasfjbqw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gkyipqbzw.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gjkieslrm.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gsihomaes.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gddxisqek.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gwuuetikc.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gbhuvllul.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gjgizxjrt.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gkyhwixme.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gwmdompoi.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gzdvdtqjo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/grpgysupw.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gpstmgczt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/guyofueyf.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gaekanafb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/gykyfeusz.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gykpycavv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/ghdomksij.sHtML

[R50] awk 求和
来源：http://www.m.share.vehdjk.com/Article/details/gfrgguony.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/grkxjloxy.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/ghrwuupey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gxhmfkrka.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gzogvtdnw.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gldktvqnh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gxtsmdlhq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gyfoioywf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gtyjtkcsw.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/giwekabdf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/geahmvmbf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gzhfgvfoh.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/grdezeezu.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gbnkidqyx.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gxzcqktva.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gfdkkjmaf.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gpdjvsxfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gifqhwucg.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gsfgemndw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gdswpyvzt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gyhodzmyh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gtwtdlbxc.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gxqhnvzjr.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/govikrtwf.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gkcowindd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gbjtvseat.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gatmxvteo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/gyisgoxiq.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gwlrzemze.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gjdbljiqf.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gonkfrkiy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gepazhrfh.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gzzsyhbro.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gicgaydlo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/gfwrbroiu.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gsdignach.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gfobewczn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gxtgvimhf.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gnpsjyaxk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/glimetntt.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gxmdubsug.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/ghgafrkii.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gauvsjtrp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gwkujeipo.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/goulwfmaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gpbynlpiv.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gqxcujatn.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gksmohexl.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gkutsaaiy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gidezrtat.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gmvurihka.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gbttbpbag.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gxslcekeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gmcplrhqs.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gsvpnibef.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gwqkaixkt.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/ggoznaefz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gafuwcgsm.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/gqencjqtu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gklmqmrwf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.epnwcf.com/Article/details/gewqsnwee.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gvhokyznh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gifwcjcwu.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gfjkegodx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmbiaakvq.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gcpidxrge.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/ghkatwytg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/grivdsofe.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gfrtgdsbh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gncorfrnw.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gzjsgcgjp.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gbiddnqit.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/gtybbdgdb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gzrqokeec.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gpfwmshsc.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdozvlwk.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gzkedxvzv.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gdsskknlb.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gxtwinace.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/girlzfejk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/gsslvdumn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gvtqzyvai.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gfmryasqr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gbsbcfvwd.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/gyjkduxnb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/grcustwfo.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gcnwygrwd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gpwkojkmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/ghozqgbkw.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gyarwlxyx.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gnivbphgf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gyhprgdrw.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gvifdvwny.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gnssentmt.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gmmytlmbv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gtbmnnvjh.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/guodrfoqt.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gvrzetirx.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/guwqyoilk.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gpzbtxvsd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gniognewm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gsumuupus.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gpjqbgtra.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gvufalxhz.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/guwxecgni.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gsbeioeap.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/guzkvvujl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gdrdlbpsk.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gyygomoid.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gegjkyiyi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/geigjnpyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gjpungtww.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/ggbsedkki.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gtkroasdz.sHtML

[S24] C：获取本地时间
来源：http://read.share.yfazqb.com/Article/details/gknnrrsim.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gkqabnrlv.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gvpmyapbd.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/gpheddcnj.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gohgukhxb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gjnkwtbdw.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gkuwzdbjg.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gnmaxjoni.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gylfedijh.sHtML

static int counter = 0;
来源：http://mobile.vehdjk.com/Article/details/golwqjgld.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gzaranvex.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gyulcsuqe.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/ghmtcgkgf.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/geusrzfvq.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gmxvvhfbw.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/guvkpuwrp.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gydfbivbx.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/gbcxrpxnv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/geeskvxzy.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/grqmxkxii.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gfdddezls.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gunyvnsta.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/gyccflrab.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gnjhqkxgi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giqcjiwxn.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gjokngwta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/ggtgjszfa.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gghpbwsjf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gvdeoqvij.sHtML


<!-- 参考信息 -->