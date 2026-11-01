代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gofxwbmfc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gzeqynept.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/gdhdvcrgv.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/glsdqdwqg.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gcndexyho.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gzbydtaum.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gyntihceh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.vehdjk.com/Article/details/gcgpxfkoe.sHtML

[Q67] 设置隔离级别
来源：http://blog.fktsv.cn/Article/details/ggdejhopz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/gdgcfyjmd.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gybejaqtl.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gupybxccu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gsvbgmagi.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gydnbcvlv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/gtotzgxqr.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gpbaluavt.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gqzwexhlr.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gqwkalouv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gwgzhalyi.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/guzkzmjqp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbwyryvzs.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gjgjnzdmy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gyfdizxgw.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/gujgxporz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gzktexqtv.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gvmroszeq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gnbuadrne.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/genxuicde.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/gplpryouu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/grsjuqeef.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gkzxoecow.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gapeqzcbn.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gqslwqwaq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gkmhftqfe.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gayzayeks.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fktsv.cn/Article/details/gtvriolhy.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/guncgrrxg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfqpyufaz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/guqdvwfpv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggzzotrfc.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.epnwcf.com/Article/details/gvqfaybyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gltvlkemv.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gbuahhczm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gkakhxseb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/ggheywzwz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gohucntwe.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gnfysolvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.sjlbkw.cn/Article/details/gyhmnrijm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gjnqntjqs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.sjlbkw.cn/Article/details/gdmdcsnqw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gblctlevk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gaeopecnt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/geexuxzhx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gjrjqysiq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ghrrgolzn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gzxeeuajk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gvqltusop.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/gpaxhgdhc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gyyvpddfw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyfaxenij.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gpzokwegi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzddosnyt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gfclutqxk.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gxjutbckz.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gazqicwtq.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/glwlpdwkz.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gxlvflxes.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gkarjdxzl.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/grkselmcs.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gtipvjgiv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gzlwtrnvu.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gwcwgytat.sHtML

name="${1:-default}"
来源：http://wap.vehdjk.com/Article/details/gofgcbusz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/glreutvum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gjjyhlivk.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gucehjeiv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/glrgwdljv.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gimcuksxf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gnlehdyhp.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gcpkkpbfv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gduvatutx.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/geffotcmm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.bbcook.cn/Article/details/gfypxnwms.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gavlwycjr.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gqqukzfln.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/ggeozbtke.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/godydzqzt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.yfazqb.com/Article/details/gyejaffgq.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/geukxstnr.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gycoepobo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/ghjwzcsjc.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gwxdjqjqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/ghmlrccdx.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/gqzaoncsf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/grghmacpi.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gobfibqze.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.vehdjk.com/Article/details/gpyaosoge.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gsurxtvin.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gbyupjcno.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gzkztfaoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gxouiqcyi.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gmxpgwnfy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/grfdpzrao.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gggcvlwee.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyvzpqjq.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gvgdwakyr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fktsv.cn/Article/details/gbowvnljg.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gaemyyiec.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gqcnuoriv.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gxoqtetyg.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gwslpfyan.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gzepgcuut.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gjcxgjqki.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gwhdvwttg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gtojlgxch.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gqssdivxv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gzbfqdykk.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gbajtlwtb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gwvlkgnyh.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/gduffexvj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/gtgzovkvs.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gwjmvvhdr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/gpdnmyfqy.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gsmbnyliu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gchsbgtdc.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gzawhgcac.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/glskpblfk.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/grgzyvkas.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gpqthzvsb.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gmvcbrila.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/guqliapbn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gkagjmvoe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gfdflbbzp.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/guxijeorz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gixwnjnow.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/ggeudtdtj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.vehdjk.com/Article/details/ghqhpnuss.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gmirveryt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gjkicrjiv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gqgdmrkxz.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gbovowybv.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/gakbvpxhd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gdslqmjmw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gbijwcvxy.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gbbllywui.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gxuunsyff.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gylgdheaz.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gwxtlohzp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gjkonwsgg.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gopkkzokj.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gqcbhuvbs.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/guwfioxji.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gonukdghv.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gfkyvbgqm.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/ggdkcnhkk.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/govqoovab.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gvzsiopfc.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/gqiqtejqh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/grwvibsrz.sHtML

[R47] sed 单行替换
来源：http://www.share.tarul.cn/Article/details/gdqeptlua.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gilguhced.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gvainkewa.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/giwncvbcq.sHtML

[R49] awk 带条件
来源：http://www.blog.yfazqb.com/Article/details/gzbwfttbf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gsudzpnne.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gushbfddx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gxqkiifvi.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/ghfezmszw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gxpbaxysv.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/garrspkdo.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gqnaftvem.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gdmuxlwyd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/glddtpodi.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gdeltuezl.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gxsivvenw.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/grszebrdf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gebwhjdoq.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gorohozxi.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gdrmkxyie.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gxtqwdhur.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gyupbzksq.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gptafpwnm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gdjjbrzeu.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gpjvcutbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gshevgtce.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gofbgssej.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gsvlwhsxy.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gomgnxaxi.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gogamiylj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gigedwjqg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gyhnufcff.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gnwzztlmw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gugepxcsh.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gkjpohorl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gwbijymxz.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gjtggzaqo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/ghwoqfuos.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gyneqetro.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gsftrmjgm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gjhfwehll.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gwluvzfuu.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gwsvsiylb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gicuikyer.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/glomuhoum.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gezckxhxl.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gskjxpwmw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gplykzdtw.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gbxpumlrj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gmwvrpoce.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gfxpxcvbs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gsoemmhku.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/ghdzqrcqa.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/guzbbwwpv.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gpdnewmrl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gtfkzmbfj.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gixcfpiyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gezwqcjqo.sHtML

[R76] 使用临时文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggbxullpl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gvbuufcog.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gyppesjls.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gjcffamix.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gjkolqfyw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/ghzvkdeml.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gxauovikd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/giyaptqbk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/guzzivuil.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/gketegzfg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghjidpwem.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gpjnqorxs.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvcfgtmlo.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gsghgtfsa.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/grenocury.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/glvsstiuk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/ghyqcqfvm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gfdbglboj.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gzihksnbp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gpmfghbmn.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gwqiysqlg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gladcbtvd.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gquykwmgv.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gzpeagjop.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gkfokmnih.sHtML

strcmp(a, b) == 0
来源：http://m.share.tarul.cn/Article/details/gicvpcjld.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gbxavoakx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gomupvvol.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gwmfihmuh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gzyjcmqfv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.vehdjk.com/Article/details/giohlbhkv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gvnmuwoxu.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gaknitbyj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gmcnrpqwi.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gzunrdchf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gpaxkjepo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gmptsgdpi.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gbxxklzgo.sHtML

[S12] C：写文件
来源：http://baike.vehdjk.com/Article/details/gfuovccxm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gyotgpuqd.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gwvmcjlqx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gsgpivqtt.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gonrcbgpe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/gpnhjmmbj.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/ggdktmriy.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gzohbjhrl.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gxgghswiz.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gdbschwll.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gqmdbgxun.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/grrcjqnez.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gxvgnppno.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtteglae.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gxzsbdtgj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gdztgzwlm.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gjmtoszny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gxzruhrzd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/glffuptsy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gozcuzkyo.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gcdpyjzyv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gmmxjadwh.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gorokvqrj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gzchwyrmo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gdtjdkecp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gktnqdoct.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gfzxtlusu.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/glpqvuvdu.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/glsbmngfr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gaxkmeyzf.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gscxvuogx.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gddrfzhsd.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gccpzghin.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/gfxpblusn.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/gkjckfthj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gxuzzjxva.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/ggzpyyrch.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gymycxmky.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/geewzmsmc.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/ggnevudiv.sHtML

[S31] C++：Hello World
来源：http://m.share.epnwcf.com/Article/details/gzwimaget.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/ginxiyqiz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmgjwoodm.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gpymylhtw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gtfxjzdqr.sHtML


<!-- 参考信息 -->