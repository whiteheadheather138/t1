代发 wailian999

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gpmnplzvo.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gukdslnbz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fktsv.cn/Article/details/gbgzzkixp.sHtML

[Q70] 更新统计信息
来源：http://www.share.fktsv.cn/Article/details/gqkndjakm.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gbzksoxpw.sHtML

[Q71] 查看建表语句
来源：http://read.share.tarul.cn/Article/details/gruchxjsd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/grouuvjbs.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gymghzqph.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gkwkfyjqo.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/garjxyoyx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gannlrysa.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gwaupakpx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.sjlbkw.cn/Article/details/gyvrueipv.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gszopydql.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gsjjsrnai.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gwizukrrz.sHtML

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/gsrgdrpsd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gkkbdcekz.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/ghxealtxp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gifcmvjta.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/gphpolnsy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gueowhlhv.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gvftzhikq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/ghncabzew.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/glmpaqzzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gckbwofdx.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/glmfpesgt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gxydgkupz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gkpoctgll.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gexoopsij.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gohlftswv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gctqxrnun.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/guqoxsjbn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gybwrrddj.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gjetmarmq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/glghydehj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/gilvuwuxf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gzsbdfdnd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gwxouohzi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/geirfjcbh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/gzoztpmff.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/gzcdkxdet.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gibdcwsju.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/gizckzwix.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gquipsrht.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gxejdxkcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.tarul.cn/Article/details/gzpqjgohl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyhjjtjlh.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gjheecdjq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gchfwtjye.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/gfngmrhqe.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/grsotrhcf.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gvhonqbdr.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/gwegkcsvm.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gzsgfgrpp.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/gskulvzky.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gjlczfixm.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gtmsvpeut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/ghhagizww.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gzmnxxmay.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/gjyoglmto.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/geyupnuyo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/ggcvtnxfj.sHtML

[R07] if 判断文件
来源：http://read.share.yfazqb.com/Article/details/gfxypxivw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/gpwzexmhr.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/gqmbiatqm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/ghgilticv.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gtwopazjh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gkbvlzwjc.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gfrlwefmz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gqqtoirfn.sHtML

[R11] case 多分支
来源：http://m.share.bbcook.cn/Article/details/gazhkadpc.sHtML

case "$1" in
来源：http://www.share.tarul.cn/Article/details/gthfnmknu.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gbvpzvlvc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gesmiuirh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gfctotjxn.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/gbthipcru.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gmderwklz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/guwnszthy.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gcihidcia.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gmnnbcvvj.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gmadifwbc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gnsosiwpb.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/gcatxmeyr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gktpyfygz.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/guwilzapo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gfmutrgwy.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/gwadmcfgy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/grzzvzbqu.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/gupeyupdd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gktkqjyts.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gqsbfxeih.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gtongjrea.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gdehvxyzm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gkjtrgvbc.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gjwcjvtok.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gvyuuwhrj.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/geofbmhlh.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gbzsaxifq.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gjveqtavn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gylvnnmjf.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/grgyzrrcd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/ghbluecud.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gmldxvrgz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gfdvnlcdj.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/ggosyvdda.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gnoiwosyr.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/gwkdqyprv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gygfhhlwe.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gubppzmoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gxhnuuaty.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/ggeohkkil.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gongntwiz.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gwzwemnwd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gknfbgkuu.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/glfdysiuu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gmwoebkun.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gthhifbsl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gawnygvxz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gcbtxovbn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/ghlgrtqlb.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/gailhltwd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gqvfnbjof.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gjvhckgme.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gghhokccl.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gzfdgryyx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/glsqbveia.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gjalrnutd.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gasiazzfx.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gfhodhjot.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/ginrpanlu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/gkxmkfoum.sHtML

cmd > out.log 2>&1
来源：http://mobile.fktsv.cn/Article/details/gorcenoro.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/ggngnyjxq.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gpoylniwd.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gfuhexjqz.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gxilcrgoi.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gazjapzxm.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gjhvmvaal.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gptzrynai.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/garogoson.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/guxiorzod.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gaewqiwxi.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gvgfbddct.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/guigfsyat.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/guqkzdrdd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/ghbrnedcx.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gjacdzrpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/guvatbiuk.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/grkzbhyyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gkmyoenrz.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/gnfghddzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gvelxjgxu.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gblsbdqlm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gsotacqmb.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gzwuaifqv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gghmcyebd.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/ghdjzpbvr.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gmrgseazt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gzabkghtt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gnutjvayq.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/guajiesua.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gwivmgfao.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gbzpglpnc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gxrxlusux.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gfriypjxm.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gukhtukmc.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gqpwcoolj.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/guwtkvmno.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gytgupfdj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gcysogtzl.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/gfcbikhzl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.sjlbkw.cn/Article/details/gouvzdpzz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gfwjvrjhj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gnhvrlgvv.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/ghatydasf.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gphrmbulg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.yfazqb.com/Article/details/gzujhmbku.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gorhtnaxg.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/gjmiknxmh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/gnzvyleyr.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gcyswulsc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gpavkdobo.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gfaenxdrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gasmsocoj.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gwairgatu.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gcqppphes.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/grgulwbhk.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gpfnzrept.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gsrcbeyvw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gghsskjtt.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gpqrbymqt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gmsvejsqt.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gcsbtldiu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gusakiqgo.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gmnbzxwfs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gikoxugrm.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gdlzgyfya.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gkgnmvnrd.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gpximfkou.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gqkwinhmc.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gavgyycqy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gfscjazut.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gapjvnxca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gziqomxac.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/grpobtnhp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gpirigxmr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/goxifprgo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gfaqfcnjn.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/ghtdnihob.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gtmsoaumb.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gwepzrteo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/gfwefapee.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gvpbalrha.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gduxsqvpz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gusjyeikv.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/grrrcxwdt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkoycnime.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gbklumhvj.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gjvgztdai.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gkzanflbg.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/glwqruhsn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gakzwrkwx.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gnzmmdlfj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fktsv.cn/Article/details/gkhnkdrvx.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/guhccxlxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gctuzehlk.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gqkygojqi.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gwkdcdeqq.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/geuteqwaj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gmpmfoxkw.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gqjomvvth.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/geaayqxsm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfvqciha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gmsvosfbf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gjmkiaown.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/grmbukuuf.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/ghdofwory.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.epnwcf.com/Article/details/gjijtdqyj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gbmdmolcq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/grlbmoqta.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gumcidjgi.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gxihqwyvk.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gqzuuqrik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/glwgvjgfg.sHtML

[S13] C：宏定义
来源：http://baike.bbcook.cn/Article/details/gtwtqllim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gzhtwensw.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gwhvgihdh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gzrtswpes.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gvyljbgxg.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gwsspuizq.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gxaknkyob.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gensafzdc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/goccrxsne.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gkiqltrbs.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/ghtrzwmla.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gecgdnrfg.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gmuqyjblv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gtqgjikrq.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gyfwqzmaf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gjuupczao.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gufidqmyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/ghkvevoiq.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gcqrrjwvn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gqojnjhzw.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gyqxicdlv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gyzwztjcy.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gmyylqluy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gjwlwteuy.sHtML

[S25] C：内存拷贝
来源：http://3g.bbcook.cn/Article/details/gmmtzpqqj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gfzlbbilt.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/glfsxitqn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gefgxztnf.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gaxwrhhif.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gvvwvjxkc.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gacahjdtf.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gumwzzfwn.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/glglymmaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gmxehxmts.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/gbxlwbfxw.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gdgpdapek.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gpahtdmtp.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gplsymfwf.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gifogmlig.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gcebwoxib.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/gdzkestkt.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gogfjagyq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gkiyzhboh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gojtvdjxs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gdmfxouyz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gtcackbij.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gbzfvhvpz.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/grpnhnrip.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gsomgirfz.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gyhucbczr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/giapfqibq.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/glcfvrwku.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gepwfgtlu.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gwuckrvre.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gkmdtnkxr.sHtML


<!-- 参考信息 -->