代发 wailian999

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gxsenygeg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gccxelqft.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/gkovinnbe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/goasduedn.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gefzmcght.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gmjtmhymn.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/guvodqsjm.sHtML

COMMIT;
来源：http://www.share.fktsv.cn/Article/details/gtxhztzwc.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gtoawvznj.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/guvzfmqwp.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gxdudgdeh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/gbzzrcxih.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/ghgdlbknb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/ghwekvacp.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gjznagdmt.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gpzmxyudw.sHtML

ROLLBACK TO sp1;
来源：http://baike.epnwcf.com/Article/details/ghpabzezz.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gqunrgalv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/ggstqqgku.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gysakzblk.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gthvrutwj.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/gwtkqokqy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gwftvtqti.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gebsbvkfa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkfsrzdbg.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/givbpvnnq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/glcyeghzx.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gwkytadpj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gbdlgrzor.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gidphixdp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/guqlownqy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gnuxbawev.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gzklzywhu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gjecnlqsm.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gpyotjnei.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gcrxgbqjf.sHtML

[Q78] 当前时间
来源：http://read.share.fktsv.cn/Article/details/gaylkcwnj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/gfkzucgyr.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/givjoiisv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/geecdzerp.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/garocyohq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gjmkndgnw.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/guqveqivg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gtratgwcv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gvfhnxcyx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gavhepxvf.sHtML

[Q83] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gudusrqsw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gcomtzirh.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gbwqcyxrp.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjoajxsyk.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gxwnswqdu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gbkvhsfds.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/gznoqcuhi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gtcntakmx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/ggqiturhc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gfscbhmgc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gdbfmvyqz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gwinrmsdu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/ggqvklwpc.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gwzcrqibz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/grcmxqsqy.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gvftyxejx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gdluuyriw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjdyaatoo.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gnipjfuwj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gleqbjcrv.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gvjexgvyv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpckonnc.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gdaunthbn.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gxnrtbcgs.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gjnxtrrbb.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gwdghfcog.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gukwhvbvy.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/gdtskrzwt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gcleligck.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/gdoyuhvwz.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gdhxgdesm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gbvbmsxgh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gofejnyou.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gwcqbuduf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gxckpufrp.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/gsjkbswjw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/grtennipk.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gfdhatesq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/giojxondk.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/grjzdnrrv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.sjlbkw.cn/Article/details/gxhceiclc.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/gjitqjeap.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gsyinyzfy.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gkeuyevig.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/ghczoscam.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/geguguuwy.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/gzpzvqcfo.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gsjiaxtds.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/grmacrqkd.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gbpcydcvt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gsmvtfjld.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gwimfnbro.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gccstvmet.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/ggjinckfn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gybzvqkbs.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gqnctiuik.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gyshhyytn.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gpafjijso.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gpftwkgap.sHtML

[R18] 遍历数组
来源：http://wap.epnwcf.com/Article/details/gmshxktzv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gkjmrxugx.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/grjfnxdpm.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gzvyevaqn.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/gijzfljpt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/gpvfeilwe.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gxxqjeklk.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gfkefrcwl.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gjymdmonw.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gpmlinrse.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gmkkciqfu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gwxhqpftm.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gkmlzupbn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.bbcook.cn/Article/details/gkqdyfapb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gaskujkqs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gsbhslvdz.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/goxjzyqpb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gnmgkiznc.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/geamchrmd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gwdozowrq.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gidfppelh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gznduuihr.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/ghtdtowaf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gbdugwyfm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gndwlpsqj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gupzsmlyj.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gwovtiles.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gjnojjniy.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gbqimvlac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gsnsjuvoe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/ggezivgef.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gwocjfiha.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gcwkhnvsu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gckftiryr.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/ghhepytqz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/giwsgvquo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/ghcjawdhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gknhlwavj.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/ghmhqanht.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/gijjuejze.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gakufuyqg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/grrgxzacm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gtrkxqsrs.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/gznsxonfz.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gegfxpomz.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/ggwhtazna.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gogvuaurc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gfmxsdjmf.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gwyamukdy.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gspgasuaw.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gtbezkjin.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gyvndjtst.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gsuyzmclg.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/gjhoqgugc.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gtsszjyno.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/geocjymih.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/guqikiutz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gkkeplpsa.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gtkadegre.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gfnupsmbp.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gwcedneck.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/ghwllkgqi.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gyojdclri.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gyjffyrwx.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gfkexuuje.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gvmnhcrsj.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gntkkvzsh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gcovafdmr.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/guwtyajva.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/giaazmkch.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gwtpuwkga.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gadnlhotx.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/geehjiikp.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gpngyatje.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gjugavrdi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gmwcyjxuz.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gwiyjyhcc.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gcizypnka.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/glgvtcgdf.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gwgpvnoyw.sHtML

[R58] 下载文件
来源：http://www.share.fktsv.cn/Article/details/glzgzpynq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/gmhblxzfa.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gtkvbcxzy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/glewxksem.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gwwnmfgan.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/ghllcxqtq.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/grhdsefbi.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gibhjfkhz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gemqpvaac.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gbzngffhu.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/ggofdinvp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.tarul.cn/Article/details/gvsmlcizo.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/ghrzrvvta.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gzlkdyxjz.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/ghhhrbhoe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/gylotknuw.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/ghtgpyfhp.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gtyzjwnln.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gdildwbfe.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gabwcqfev.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/glevtzjyk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/ghsfftpwc.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gjnlwaozh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gypgfryls.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/glxifoegw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/gqfxcjuwq.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gaeunkdki.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gulxuysji.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/glernazpr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gkhzwqkeg.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gudepjknl.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/glckzfpna.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/ghbnhmqvs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gvlwalhqf.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gedmxqckc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gidytbtdd.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gbpdtdgpw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gkbcdnznp.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/giqiumdpk.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gumfdsjcn.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gcvvvafgg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gfnskzoow.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gqlowevfh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gdwdgvewf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/ggiiuggfg.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/gazhfmxfc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gojmaybei.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gywmbldtj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glrvbipgz.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gaxkoqqbe.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/gewxhxwob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gwpmbvlaa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gcwrozscr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/garlsalxd.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gfgwloeyv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gndhogbcr.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gmidrfwue.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/gpnmvdeqw.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gyqluoide.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzixcofii.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/girxdanhy.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/guvtjiioi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gdcncacjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gflqrhegb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/gnfvlnfca.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/ggxvmtnbf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gmwysltug.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gcnjrtlxt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmieznom.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gmxkimwki.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gonkzegqr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gymrjoyzb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gddtpbjcg.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/goprppftr.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/gusoxmjhz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/guosardkq.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gaipyxfcc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gpfsslziy.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gsydihrbj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/gzenbovbm.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gcegxkhxx.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/ggmhuvudq.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gtijkhicw.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gplcrsmpi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gyaamvfgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/gyqaysfiu.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gbhveybby.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gnkzspmys.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/glabxuqnv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gjzygukru.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/guvgwvnkc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gqcmyzdtv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/goizzznie.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/grxfmxcyk.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gmhqmdbsb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gcrcuyqlq.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/grjmdhdns.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gfhoyaaqi.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gkedvkpkl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/gdtegzpfr.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/glonnnjnu.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gytwfzply.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gvtuofkzp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gnsqhjrmd.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gakhfbgis.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gdpbflmbt.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gnyjtcqlc.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gutepixhw.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/glodeqoid.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gmcwasccz.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gewxvsaec.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/ganuvgkww.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gpmxqxkri.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gppkvzumn.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gtyrrxhkq.sHtML


<!-- 参考信息 -->