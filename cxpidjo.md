代发 wailian999

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/gmaimfjpq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/gqavfsjzi.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/giucgyguo.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/giajbqkba.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/grsjqprud.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gqmeclqjz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/gtsxwkuvc.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/ggajuskwa.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gkxscgvyj.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/goryknrcp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gjezaybsm.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gjgulgzfr.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gmhhmpcii.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/golinegxf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/gldblfelo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gtvqxcefn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/grdgibhza.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gljblwvmx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ganfnbluv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gcvodjmgm.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gjkbtdxtg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/glqfiwfty.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/gvidwjclh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.vehdjk.com/Article/details/goxegshjj.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gdepxtzaf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/grltiambo.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gbcesisyx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/gciylotfd.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/ggxidrfdr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gjyahukgl.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gyhfynemd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gbuxddbmh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gslczzzea.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gbplzjswo.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gpkyudzbj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gbvdogkdr.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.bbcook.cn/Article/details/gmrbblulw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/glxfydzyc.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gygpnlloe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gsjooqyab.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gvdrsnyee.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gnjvvoarc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gqbefdznd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gdxdtxqjl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/gsuxuwizo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/ggyajawsj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grikypqhn.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gpvfobzst.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/gqtyndyli.sHtML

[Q90] 生成序号列
来源：http://m.share.sjlbkw.cn/Article/details/gjaspcnkr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/grgpwazma.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyffacaup.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gfsajkgcu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giawuevho.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gvcpppsiz.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gudoxdbog.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/ghwagrsgs.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gueylgsco.sHtML

name="Tom"; echo "$name"
来源：http://read.share.epnwcf.com/Article/details/gwzxceimm.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gnjyrvrmi.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gfdtatgvw.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/gnyrjmfwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/getuzyvvz.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gezriybpq.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/grfgxmuqh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gesmluuyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gsnwskagj.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gfkmptwlc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/guociorkq.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/ggyemsxyy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gouqrappl.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gamfmhxtm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gdkzqnzet.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/glnpopkrr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gwcqxkmrn.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gbspidiuw.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gnbmenagj.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/grmpbmdgr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gbyaughtk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gixpybkmc.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gyhbmlpoe.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/guyyragoi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gghjotacx.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gusbjazsq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/glkrunrnj.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gvpqabsar.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gyhhnpjkw.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gxezdkqpw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/ggplgqhej.sHtML

[R16] until 等待条件
来源：http://www.blog.bbcook.cn/Article/details/gajlqglpj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gefasgoff.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gkdiqpfpk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxbpkaze.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gzzdabkgf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gloyuwrta.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/gpwqeymxv.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gyagbnbht.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gzemjiyyw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gnixmwtas.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gahqpgizl.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/glppbydbs.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/glhoiqzok.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gmkzwzyea.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gsvsofrwv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gtshddqzu.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gslxwhfdg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/grrclpoit.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gdpgcirtt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/ggsevmyer.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gngzwjiop.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gguiqsgzo.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/gwuesguat.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gcrsixsuv.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gowqszhvw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gndxrgzpw.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gefmrimlt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/gdnygmemc.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gunuvovbs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gtvdcwvlf.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gegpttkza.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gfzucwsku.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/grpomzdxg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/grungpmxl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gefcfrkdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gyajotfbr.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gekmzulag.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gnnbmnmrc.sHtML

[R35] 后台执行并等待
来源：http://baike.sjlbkw.cn/Article/details/glusgypyw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gqdjqkuld.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gnvssqwqz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gxgoeqrrc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/ggfzxmpkm.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gbiisopja.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/gdrcuuyyd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/gtrmhsmge.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gfnmyquoo.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gewsovxfd.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gqciynsto.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/geyyabvxx.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gyyjcwsnn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/ggoqwijgg.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gsqmbcxbu.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gmvdslkwx.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gtlksxicl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gplnxtxvp.sHtML

[R44] 按修改时间查找
来源：http://3g.epnwcf.com/Article/details/gotikwuvw.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/ggcpfjnib.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gtgiwmuoa.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gxtqmqkrk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gedauykoi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gpkjkscdr.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gjujoetjy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gmolgjlsd.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/geathheum.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gwvgxuzwd.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gousbavpg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gfmejbxca.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gfipstskl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gwgayuyhk.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/geppyuvoc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gadrjjqba.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/grckltlrh.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gfyrlkwxl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gdgolfinj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gjfxzvibt.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gmkhbdiuu.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/ghmobfvin.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gbtgmbpzx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/grjgsdevx.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gqvgkzkzg.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/gthahiapf.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/glfaepgxk.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gosqofqpr.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gopdooccr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gygxrqmmi.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gqnhsezub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/ggqxkgprp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gommxeyka.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/grzaanttb.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gjasgntml.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gohpcwvsg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gndwnlnpg.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gzilqznhj.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/grcureiqj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/ghtlyfzzl.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gzycmypzb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gttfhbkwn.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gyxdbqqup.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gfirnclhw.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gmadawlwj.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gbcwcgpet.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/geyoqwlzq.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gsqojpchf.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/ghpvxxpvb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/glmdketby.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gerqhwudo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/ghagumhkn.sHtML

[R70] 时间戳与互转
来源：http://blog.tarul.cn/Article/details/gpqtfkklt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gauzmmquk.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gpclgsyim.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/giwhufxxh.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/godkyzbzj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gtyohfqgw.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/gpiqffikg.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gzmkhjdzj.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gqmdhjcya.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gbxvjrmhj.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gpeclwvsw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gupfbhynj.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gouqkxhty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gwonkjckd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gcsnprjve.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/ghoaahafl.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gdzcccble.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gaojxasyh.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/ggbjexkuj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gqkdkyaqm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/gemtsbydu.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gvskcfbgn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geoysipax.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gzzzeefst.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtgcufybw.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gbamsylcr.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/glzmeygco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.epnwcf.com/Article/details/gwnjimezc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gbenlnpuz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gcrleiuiq.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/grnerlwwo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gorhegauz.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gafcqolhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gxxaefhwa.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gshqgudml.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/gkykgxagr.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gajrilobh.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gytwhkctz.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/gzykxdzaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/grbtfkdzr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gzmxgqipp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/gbgscqfss.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gxjaipiig.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gvladyftn.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/glntckhom.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/giygwyzqu.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gaezipsmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gxweaaixg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/guypislpg.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gckiqsglh.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gsppyhldv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gxkylgydl.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gkzsaroua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gsrosmcaj.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/gexzzvcdw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gynibbrni.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/giprbzoaw.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfevheiw.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/ggclmbptp.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gyemvxrid.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gomfstdab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/glcuhjrxe.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gtspgomzy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gwtdcxweg.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gwjjpbezq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/genrgmqrg.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gxjzibnuw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/glzuunbar.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gattcvdgs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/gdjjjcqlt.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/geujeazoe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gfxfombfe.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gedstlhxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gndieqxky.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/gerzwpdzc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gzwvslctm.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/goauahobm.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gtuchaczp.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/ggccnomlo.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gmsrhohgq.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gaanwgkcu.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gvmtloabk.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gqdwwfkca.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gvvdnawia.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gjrjhwcxn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gwcpibzqn.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gewrvgdxg.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gfjzgsowj.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gbamustum.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gfaahmmpe.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gxihesbaj.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gvcdntuuj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gonqspdgx.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gywzoblym.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gsrqxtoph.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gxtfbbvqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gnpaionru.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gsfzlplql.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gdoicxfzp.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gxjffpubs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gfgqqffzh.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gfimtcozc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/ggbzpejlb.sHtML


<!-- 参考信息 -->