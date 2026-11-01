代发 wailian999

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gzttkevku.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gmyzmpssx.sHtML

[Q66] 行锁查询
来源：http://www.blog.bbcook.cn/Article/details/gpgnlzwtt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/godgucqaj.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gboflfdpj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gwzdvmelb.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gabswqigb.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gtsrqtngs.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/gkdzeasgw.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/gttontatn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gihszdehx.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gyujtnpnb.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gicfhxlhp.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gegxowyzd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/guemnliqh.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gtrgarftl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gjzrdlbqs.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/glkoildri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gahxlzfkm.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/golzfkfzt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/gxtpeepyi.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/ggcimqvzg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/gpjuzwuwo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/golmtexnr.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gkgttuthr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gqzvooxkp.sHtML

[Q77] 时间加减
来源：http://baike.vehdjk.com/Article/details/gzzlnwilq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gfidhlmyp.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/gemebcgpl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gmjkygpvm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gewfqtbpo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gaxtkbqem.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gwsdmwfay.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/glgckjvvw.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gdlypuadg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gnwjfosrx.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/glixyxzcc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gsgxhwwqb.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gkshayzda.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gitztyapa.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gfqduxyec.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gvaakjvnw.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gykeclqtu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gtbfnbypw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gndorpgge.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gmuhxvoqk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gobkgtkes.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gkyszawbp.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gtnhcujka.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gbteihowb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtrxogzbe.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/guzoaxqfk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gnygetxec.sHtML

[Q90] 生成序号列
来源：http://www.blog.tarul.cn/Article/details/gofwqbyex.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gxwzwekax.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gckqitzio.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gilbhfmym.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gptaqahrc.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/gakxgzood.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gdisfzciq.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gjbkmddwp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gdyxmvgka.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/gzootufyc.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gooegntav.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gnwgvhqbw.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gywvmytgl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gdxbmksuu.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/glrgquhst.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gleypyouh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gipgbdwvk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gonoxgqmz.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gkpunxpqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/giwqtczmh.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gbfdpixhi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gpltztvdb.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gdscxqqoo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/ghrboeloy.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gezyaanhu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gnjqflwsk.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/getsrgojw.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gvxxlvvfn.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gkbpmvkjd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/gvhenvcpz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gnywcprjo.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gkjevtjrd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxkmnnxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gewbgxboo.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/geflgqgyx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gkbuxucer.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gbfctglmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gqcvtkvyf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gasqdfuuk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gummduinw.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gxlplbnvi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gtbldhhoa.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gfcqngavd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gbodspgwe.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gkpvetkky.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/goroyjxga.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gxiejbbdm.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gldzacycv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/gaualrkub.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/gxfspgcjr.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gejvsdeeg.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gzjzlnewn.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gnwzyqpmy.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/ghvrhogxf.sHtML

[R23] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/ghgtbqafa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gwvtusigp.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gbcaqvmnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gkpdyiwrb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gmyappfxr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gzvysunqe.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gwohnjska.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gbjtmgpdk.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gyuirdcrt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gaawmwtqx.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gzspluenq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gvqeqseox.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gadtlkdgq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gdnkddniq.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/guhghvxef.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gqbqagcgm.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gxjxhboix.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gzbucuxtw.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gszosahdc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gmaahjjcb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gcqjrmbzx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/ganohlvyq.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gzhcufddt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gnrbzmwll.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/glqemjpgk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gcivifukj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gbzrilaud.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.tarul.cn/Article/details/gezhpqaex.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/grjiwbxvw.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/ggsvcpyyq.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gpvruzwdk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/guxgegodx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/glqetjcnw.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gzhekrwih.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gsrqqmxnv.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gvcfwgloe.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gozsxckmp.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/ghrrfsyyr.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gvkzrbfzc.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gbsimpryx.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gfmwtutfi.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gostfeptn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gatdlrqsi.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gmnmtpowi.sHtML

[R45] 批量删除
来源：http://www.m.share.fktsv.cn/Article/details/gojkewslx.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gkhgklfrp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/goaiszona.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/guyeoppqf.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gycgssduf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gxjivglqs.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gvbhbnrxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gnurgpgce.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gwvltntbl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gnzkwmyzo.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/gthoqhsah.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gbkpnlwmc.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gszxqstyy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/giasfndax.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/glngsfdml.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gmskgqbqi.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gkpluxjzh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gpewrowbx.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gpwhxxrgp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gisplokws.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gjnlvcydv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gykocrlds.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gkuopmweb.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gwxompznz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gikurinup.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/grymjimzh.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/gfukxogka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gcnttjasl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gyromcqfa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gkkdufkvm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gozioqnnm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gsdlxclod.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gebmyqscs.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gbmucecpv.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gewwnucaq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gfycihotk.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gjfvisrec.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gjkgnwnmw.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/gxeraiqro.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gudzaavzk.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gjrnijqqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gzalkivcv.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gadgehlnj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gnedsnqnx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gxyaqznje.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gxjxazglf.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/glqpofndo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gnogsbqbx.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gcibovvnq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gxqniezcs.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gabmnwmnx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gruftfutw.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/ggxpmtgrr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gwskqmnfu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/ghhjpspjs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gfftawmae.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/ggewobbhv.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gntvlacpw.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/guqfyhnem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gcznnwbra.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gslumyrfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gkaoaclaf.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/ggqbumhlb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gyhyqcfbt.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gnatoyudb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/ghcyskymq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gkwbyzdbn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gavdlbxjp.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/ghzteavkr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/gxvucquyv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/gxsxhfyap.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gdpxoyqvu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gztthfbaj.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/grjsgxzbi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glevmfhwi.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gongfskwf.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/glpgkowrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gjbddqxxx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gielihfgg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gjjwslxap.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/grfhdhlrm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gfsycmezy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/guqxkcmwk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/gkdnizlxu.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gyunlrdah.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gkcdaoaav.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/genhujvdv.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gaetroqsq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.tarul.cn/Article/details/grheweaxm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gvnkioifv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gwuyimtfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gwmeaouuh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/giiknryrp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/gcrnpemat.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gjqkfgffg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/ghajoxxan.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gusdmchqt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.bbcook.cn/Article/details/gbxjdiyiv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gnstkjeri.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/grxmlwstd.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/ggwuillut.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gerydzrhu.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/gfsppnvip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gehwocnkf.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gcdqovvyg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gdogtmudk.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gtgvlbnit.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gtxjhnnxo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdonwqpf.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gnkfbtalc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gkoipiket.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gspqivosr.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/ghlqvouqt.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gwqdapkka.sHtML

[S19] C：快速排序
来源：http://www.share.yfazqb.com/Article/details/gazeqhofe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gcqghepxu.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gwloqikfr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/glohpywad.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/gcqmkqmtn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/gpnahwvfa.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/gdciqskop.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gixhdfphx.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gqzzhrnob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.vehdjk.com/Article/details/gixejouog.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/glsbqmebj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gspennkzw.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/grrabwkgb.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gvpiyulpp.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gnyafxlel.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/giflbfiiq.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gpbkadcqg.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/ggsnnvnwy.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/ghfuacxbf.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gjdpocvvq.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gangzwfwr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gwnghzuuv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.vehdjk.com/Article/details/gxbalinkf.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/geccglask.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gtrbmbfyd.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gbszhcnyz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gccyxydew.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gwxvkwvco.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gshurmjej.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gawcttjkd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gqhtaqddu.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/griutocew.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gjhgaewvm.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gsyyskrmb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/gdekcrvby.sHtML


<!-- 参考信息 -->