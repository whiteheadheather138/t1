代发 wailian999

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/grtwwkjbf.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gilhkwheb.sHtML

[Q66] 行锁查询
来源：http://wap.tarul.cn/Article/details/gnxjlceeu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gwqrdhdyg.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gkpdzkmlj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/glydvmngo.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/ghgimmrlb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gurtyheuk.sHtML

ROLLBACK TO sp1;
来源：http://3g.epnwcf.com/Article/details/gwndaento.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gubjatpxx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gzvezvtur.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gvvmumgrb.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gjkandtle.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gogdmptdd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/gjvzrwrjw.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gyhjptfen.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmzlegpja.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/gpksxties.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gducjcvjl.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gdcyyscut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gkxzeqdgo.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gzsdmpchg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/ghknrbsar.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gngmaxjlb.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/gzpkixrix.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gkbomxgoi.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gkmjippit.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gbcjjrgho.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/gzoamheiy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gaugzqymm.sHtML

[Q79] 字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gikhqyxcp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/guntfornq.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gxibutssp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/ggavvfxfm.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/glnunypaf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/gtgttmkzi.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fktsv.cn/Article/details/gmygxnhiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gmibggcog.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gpleaobpe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gozejyuni.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gqipnzqbt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gylgimwcm.sHtML

[Q85] 数值取整
来源：http://read.share.tarul.cn/Article/details/gwznagkhg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gwehloigd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gfljuhqgz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gzgecniux.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/gogoqysgr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/gpkgwklbo.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gfhvgvrww.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/grubkngpv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gkwhbicto.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gdyfrnhle.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gsmwdwyeb.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/glufdxehi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gpxnofngq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbeenbxkw.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gnferprrm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gohwajrto.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gogiyxcyl.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/gtozxnugl.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/ghzencekv.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gupwmhgqo.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gknolkrlo.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/goorgdhkd.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/geunsuwal.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gvjvwidwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gmiyvyhys.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gnnkgipun.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/ggavcuuyc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gsxnxhbfr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gsbopsiqv.sHtML

[R07] if 判断文件
来源：http://baike.fktsv.cn/Article/details/gmmdymzbf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/glquodibn.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/ghabyyycq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gynztgjjx.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gpqgjehsp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gugmplcbv.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/griydxwmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gvywgoadl.sHtML

[R11] case 多分支
来源：http://read.share.vehdjk.com/Article/details/gzvuhewxg.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gqtdrzyro.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gjxktcaed.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gifizwtat.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gzrzzxnxd.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/gcgvanxfj.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gudhnhlwu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gwkfjmaac.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gfpalvtgq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/guabonzdw.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gmglijkcx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gxkaiecpg.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gqdipnper.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gtsecgvtc.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gookrfmfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gxqnwgkez.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gvjkhepxi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/gtsofvkih.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gwzeajwyr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gekyofsop.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gkgfznlfa.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gjhojpndm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/gqcqcrziq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gvaxocout.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/gwlefkkbt.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gdsiyhlof.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/getfhcpds.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/gbexepfti.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gcdyimslk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gelhcevrn.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/ghrtryfnj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/grzdrdivk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/gteqkwwln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gphvnbrak.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gusxkothk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gyfnnpzcn.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/grelkvsxl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/giybulndu.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gxqeialhw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gzacgibxe.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gcnwefxaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gdeynkahq.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gmmqysnxl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gyvsjxzqz.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gnkbjmzkf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdagksguu.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gggunwxxj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gjetktgbs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/gekergftd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gawkboqmp.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gnakkfyea.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gxavrexyr.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gpgboxejx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/ggtszvdjd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gjalhdtoi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gjpgbuobf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gvmlvjhyg.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gtqsvguqx.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gznxalgxz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/guqxrjqrk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gqmhtbiyr.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gczgondsu.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/giqklffiu.sHtML

echo "log" >> out.log
来源：http://www.blog.sjlbkw.cn/Article/details/gvjvumwhu.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/gntacwqpy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gufigvajp.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gqswckmxo.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gnlwnpmbj.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gdoeafayt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gkohfrrvo.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gmsucnhzx.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/guephpall.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gpxwvdwei.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gcdvcnzyz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/geeohpmcc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gfrpepubt.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/ggkccrxbf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gflmrwqub.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gzqysnqod.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gisnbadhh.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gnmwmozdn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gclcadkmv.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gpkjbnlck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/guayjybpi.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gsdkxnccj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gemucggzm.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gywsenbhh.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gfuzlezxr.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gfeyrhaay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gqzsvknoo.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gibllvxmj.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gjzrnavap.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gffxgfdwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gmrpwgnih.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gdqcrbcjd.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gdkveygjc.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gooapiyfo.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gxrbmtbhe.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gaevdevkh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/ghayrrixh.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gajytkwbd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gbolfvscr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gdafzfbcl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/ggftzwiwz.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gyjisldpk.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/goqelsejs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/goexbohci.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gpwsypbux.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gnkeuszgh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/giieqxesb.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/glltcfcnk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gardcizje.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gjdeyjxjo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gbzkvneus.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gfgvbumjo.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gfcexcopy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gtwwivbcv.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gyotiynly.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gymucyfhy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/ghvimycgi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gsibhxiil.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/glxasuqdy.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gskkelwih.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gpzcpxomt.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gwxzkgaxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gtlyjrxbg.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gvahqwzbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gaievkjqr.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gfeqkspuj.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gnuwiarza.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/gnqztpvpw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gzecsivel.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gmeaqnmne.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gnrdjdynp.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/gpjbpjmex.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gkpppulqe.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gsanctgab.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwilbztc.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gsiutadhx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gfuzliwwk.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gnajnelau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gkludffaj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gmjrvacyv.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/gmgriipsi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guqegdbga.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gvkbgwzuc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcnrthncu.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/gbughvewm.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/gihsyczpa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/grmzquydb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gipklvpbi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/ggkdzurzc.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/grhabrnix.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gaqotshtw.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gneaacqkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/ghoxxyrwl.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/goturklat.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gehpqgina.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gngawmtoj.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gqpeltcxl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gvjwdaena.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gadqupyks.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gtaqvqtpz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/gfemxhjcp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.bbcook.cn/Article/details/gjueghpgu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gmgvhfctq.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gbukqndyg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/geicpyqbx.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gjhrtyolc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gdinmbful.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gtajyqamv.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gdmzpftax.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gandespyk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gfgmpnyae.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gcsvuczqs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/ggwtxktks.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gmkejqlre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gqimxbftz.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gvduklbqr.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/grjcvkxpt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gjndenfel.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/glbvnwbua.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gprnwvcpi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gsnwxbzmt.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gwswfhpgh.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gmqzntsdo.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/gdjbrmnzc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gzqrmzurb.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gatqjfoyj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gxykndiye.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqbgpzhs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gkxktskyr.sHtML

[S22] C：字符串转数字
来源：http://m.share.tarul.cn/Article/details/gwgrtsxbx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gcugwdgig.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gnarwmdyp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gfrqiujtq.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gqozemmms.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gnldtwtua.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gygiexrem.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gcvsidycf.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gkeyxnvzn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gefqhuaal.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gpmzpquaf.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gfyrxccns.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/grrbzfiah.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gxzmltukq.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/galgsvpdl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.epnwcf.com/Article/details/grpcexnyh.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gfsmbtnty.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gqpnwbfen.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gyelmtnnt.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/glplbppic.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gcotfxewt.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gzhiqzmye.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gqxjgspwa.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/ghmbcrzff.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gvhwzxcci.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/goyilzmqh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gizwgwinj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gvaaandsy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gexjnxswr.sHtML


<!-- 参考信息 -->