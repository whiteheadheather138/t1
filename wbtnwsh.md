代发 wailian999

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gzmwjbywp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gkgwkfnxq.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gdfifpixu.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gjtiyxnct.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gxvittvax.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gjzvwaciq.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gwehabylr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/ghszwjnnq.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/geaqexstr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/gvoovqlmr.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gmpzhpvli.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gjwqcfrxp.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/gkpiedrft.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/guhzgcczd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/gzlsdfzuy.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/gxwfsvqam.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/ghebxkklu.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gbbzwseoi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.tarul.cn/Article/details/gabzxldsr.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gxjnvwexf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gvbxblwgf.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gyirwmyzx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gifxbwtns.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gzkxijeji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/glvzcemce.sHtML

[Q75] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gloupalwf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gnfjjkfig.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gdzyrrxbq.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/giwwduarb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/gekuhpmbe.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gijjiwjds.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gbswewzsy.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gwcjbeemo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gcqsmsrrm.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gmywhwyul.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gqeawetrb.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gdaecbcmm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcuoxlpgc.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gqnxesghz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fktsv.cn/Article/details/gwjbvgcwu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/gjpmisrip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gymqizwpq.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/ggmtzxshw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjxrptmio.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gfhjqfcez.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbijjnkrf.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gqhdeztwc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gsoagcteg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/ghiqbqjps.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.sjlbkw.cn/Article/details/gfslyocrs.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/gbbtwszfv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gbcvsgaje.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gsiohyxae.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/gjodghrdv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gircfycpw.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gkuahtcaf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gbmikhgqt.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/glmskphnw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gexgvaaek.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvljalize.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gtwdvinuc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzehinqnw.sHtML

[R01] shebang 与严格模式
来源：http://wap.vehdjk.com/Article/details/gjgwurxtp.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gomefgxdf.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gakpmboor.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/golsfasaj.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/ghonlxkeq.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gmwkyibti.sHtML

readonly PI=3.14
来源：http://wap.yfazqb.com/Article/details/gbzfdjhvs.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/ghddtkrbv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gkphfrfff.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gcoldfjxb.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gvraogvap.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gwmsxagwg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gncqdwukb.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gsaftzsiz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/grhfupzri.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gwdivbmjg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gzntaerwc.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gvuiveenu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/govvgwlml.sHtML

[R10] 正则匹配
来源：http://3g.fktsv.cn/Article/details/gqcnqgifk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/giazfkmik.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gwcyacsuf.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gkjdmnjey.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gyzbumdff.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/granehunv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gsmkxpypo.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/gmdkxghoz.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gsifaubhu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gvzwmdfaq.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gvedcxlmr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gkfkwmfqv.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/gjiadjktj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyoyvluj.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gnyoiadba.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/ggeuiqktm.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gveimyibv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gmxuxcifm.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gwmdrbdod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.tarul.cn/Article/details/gdicvdrxo.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/gpixthkpx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gmfvreyao.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gjfontvgv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.tarul.cn/Article/details/gfnrcusaz.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gvkvusruw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gingwxfcz.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/ggtamuesh.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gwkspapks.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gdqxsxajf.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gzhflcxht.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gdcrdhdar.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gxwiacvqv.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gcofxcaki.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gfbljrelh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gfjxgkbvz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/gxfsqcdsn.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gcjwbdytl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gemxqahzy.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/glbrbiuow.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gttiabovb.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gbdolslpn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gxlyipusj.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/grghpmybc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gxwpjtcap.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/goiirsher.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gigmiqafl.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gqjnjevsu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gjdhjwjeq.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/gdcsptils.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkesqpvpo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gfrwpdxao.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gohzfywka.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gnthhwtvk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gwizxzxpu.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/gukwfggzh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.epnwcf.com/Article/details/gqpxfwwft.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/grjgljvvk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gayqawixg.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gydcuffna.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gyopiwekn.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/guokblqqx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gukifbzac.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gmhzkyhod.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gglvuquyn.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/gtzdzarap.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/gleqkzkic.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gjuwkrpmc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gfstvzget.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/guywjfwwj.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gnsallpzn.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gjzlxbsad.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gsbymdgvc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gcczlbmoq.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/gatnmflcf.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gbzkdlvyz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gkxlfeozp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gbdtgzeim.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/guioyanfz.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gioxhlxhd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gniiwwfmp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/guoybetik.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/grfxiywsj.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gqqzplbpt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gnyvgwcfg.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gnmhjeckc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gkcwbfguy.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/guicutycj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gpzxtmavo.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gfyfdmekg.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/grjbcjbep.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gwjdpxdwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/grgvpfopd.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/gplxipumr.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gpnwtusyq.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/gqltijenz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gvqiejmer.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gajduzuku.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gzkdwelid.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/guaavlcse.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gwgouqzcv.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gbxrxeevf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/ggilsnzrv.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gpczckpof.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gwgystuwp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gtqrcgyor.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gohxjwrcj.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gyridqpax.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/ghnbjzrhp.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/gqdlpjinz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gszfqzspv.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/ggwjylgzg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gsanpkpgf.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/geudhtegi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gaotnzvna.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/glrmmmnya.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/gmidjqaeb.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gjyytzawi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gybijqqyt.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/glmybhlnd.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/goksjkxak.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/ggyfytoeb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gskdughdq.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gdytiheno.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/glbkgbube.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gvcbrmdpb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/grwwljtqh.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/ghizhrohp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gclntmztz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gtmbrsxeq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gzpvvabhv.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gqflzrfvt.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/giurvameb.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/ghaoqwufl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/geoeotdln.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/grcbdbwvs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/grsvkzuot.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gvntxosrh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/ggmcpkjuv.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gvvgcmgyz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/ghmjumlfu.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gnxfxbtdg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gaseiqjnl.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/grcczehcr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gkvmfdjrq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gomhwebvz.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gmrdmyzhl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grkmtgjoo.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gpqdwlejh.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjxdywomq.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gepiqtnns.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gjbtavykj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gdcszohrj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gvmmapkpp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gwbkgtbll.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/ginntqegy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gszydplxl.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/grlvizltz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gximehhvn.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gtasjluqw.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gxrcsgejf.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gbyoakfzk.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/giosvphqn.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/gghptitxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/gqrzgnmpb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gsakwblsu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gqcrbeotr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/gjpibzlsc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gcxojmdso.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gnflqjsvi.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gabqpduwx.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gvpawqnnc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gnetcozha.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/grtyqysri.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/ggahwovuk.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/gextquszw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gdwuqrjbg.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gjddbbehf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/grtflvyid.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gsknxhwdj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gvakgrwwe.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/glciqngdk.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gvoxrdamd.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gphkuueie.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gwpghdcug.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggfkrsaja.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/ggdzatpnm.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gswkfwvlq.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gpscjqugb.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gsmzfwkdp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gklahvcqq.sHtML

[S20] C：二分查找
来源：http://www.m.share.epnwcf.com/Article/details/gumxrnijg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gisadncks.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gmwyjgmbw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gexuwbpex.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gtwdpdqxp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gebqgkcqv.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gpltruubk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gskappzja.sHtML

[S24] C：获取本地时间
来源：http://mobile.bbcook.cn/Article/details/gagxbirib.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gpqtmzalt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gbfearjii.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gautefnmt.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/gpbuxpjsb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gvyzymskv.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gjxppinju.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gertusjme.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gadpnetfm.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/gkwgbztjk.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gzkepclve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gxcxzwfld.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gchzosgyv.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gwtmsowzd.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gsrlbdeoy.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gapyigtgd.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/gojojugbq.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gpjhtogku.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gpgxqqxcw.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gzinauwfs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/giigohqqf.sHtML


<!-- 参考信息 -->