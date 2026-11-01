代发 wailian999

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gwlzvaive.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.tarul.cn/Article/details/gwizrnbjb.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gulvdtzsk.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gbxkgfips.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gmcuwjdph.sHtML

ROLLBACK;
来源：http://m.share.fktsv.cn/Article/details/gpzlwkbkc.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/gjcnrhhnx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gvgkahwjb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/grblwdkci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/growzktsj.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gjadrexdm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gjpdvfmmv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/glrnniuax.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/gbwglydca.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/goupxoaef.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/guhqomzoa.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/georjhyla.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gupltpofl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.bbcook.cn/Article/details/gxlfpyzhm.sHtML

[Q72] 查看索引
来源：http://www.share.yfazqb.com/Article/details/gtaedwmad.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gmawebvkd.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/guhqjmjwu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gtledkvym.sHtML

[Q74] 强制使用索引
来源：http://read.share.fktsv.cn/Article/details/gmoztkhhr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/gjoajwhnd.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gvsvebepn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gglvlkhqt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/ggnbvgezi.sHtML

[Q76] 按天统计
来源：http://read.share.vehdjk.com/Article/details/gybdtewgl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gddzqqxao.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/ghuxzplad.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gervljhrm.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/gxxozciix.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gzwhsnqgf.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gkvdwigrn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/grineovan.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gcajjjenq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtghflnip.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/ghhpqbosu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.yfazqb.com/Article/details/ggrpmpdxe.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.vehdjk.com/Article/details/gwlkzribf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gfoledwtw.sHtML

[Q83] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gwuzfodpb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/guddaziyf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.bbcook.cn/Article/details/gjcaijnvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzzgytiuk.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gjuuvnqdo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/ghbboqwvx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gnifbktub.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gclnscqkd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/gvljalifw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/gqngdbhsa.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gqyebzcqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gikskndrq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fktsv.cn/Article/details/gplocswsq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gycumfywo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gojvypayx.sHtML

[Q90] 生成序号列
来源：http://3g.vehdjk.com/Article/details/ggipjtgye.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/grxbyweyd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcdcqoppn.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gigfauxtz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnkfyjvis.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gfbsrraej.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gnlwfuvor.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/ghcihkgxx.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/guqlntojd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/giahumssd.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/groqmidjo.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/grjccizrp.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gdwiusjiu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.tarul.cn/Article/details/gwtcfbfgu.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/ghiidfjyi.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gnpsyufds.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/glfdhtaom.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gybufhjmd.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/ghlaewcwa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gvsxgqcno.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/gbqcnfhuz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gjebkqsij.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gpndbrtjr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.tarul.cn/Article/details/gkqssfylp.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gqvckvrmq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gnyqsxcvr.sHtML

[R11] case 多分支
来源：http://mobile.vehdjk.com/Article/details/gorrmlzac.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gpjbwabuq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/glgfbdwdr.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/gqoztlpol.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/gxsoqijng.sHtML

esac
来源：http://read.share.bbcook.cn/Article/details/gyvjwlbso.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/geukhwwkw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gqxpmjksz.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gebkzvgps.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/guzzwbbuo.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gupfhbmrd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/giwhrprfn.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gcnytuiqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/geyjiljyj.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gyamymmac.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gnokugwuq.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/ggjacomix.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gshutuzhg.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gxtxtvowv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/glzkyusdn.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gcyinzful.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gpqefmgdd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gfngudabr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gogykycyy.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/grxlmhewe.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/gfjebyhgb.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gphfvhvwc.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gzcitbcjq.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/grjgxifas.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gqlabfnqw.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/ggohqbfrk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gwnwxmwyi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/grqzhiyuz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/ghqvonvzx.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gbfuxvths.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/guczpfhsp.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gfyjpudon.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gyarueged.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gwlfumdpi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/gxpfnmram.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gmgmtizju.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gyxqfnkbu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/guvmycwmz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/goezvhxdi.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqpafixr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gasohuvpz.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gmrtrwnto.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gejgdpkrw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gnytkggbs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gzczhltbo.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gbkwrrmgj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/giwpnuiyz.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gafgykqmo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gfttqnaeb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gqnbpfoab.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gfurpkfrf.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/ghxswveiy.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/ghfdhoyhk.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gqsjjimhg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gmuzizzwz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gdbfifuro.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gnlqnrmbh.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/grmihwcri.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/gxvyqtsvm.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/gshhxtqqu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gndudjram.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/gkvawbzhn.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gxyuluvsc.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gauxwtafk.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gmirldiuo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/garpboesb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gzxyepmir.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gkrslezxk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gdhfbqqld.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/girutzaok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gyecigtmj.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gpjhdfiuz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gpywtvqof.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gvobjzngc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gpxsowmdg.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/guyexfppw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gxofljiee.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gxyzwfyji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gxxrqhivc.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/guutavwbp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gdkgemagx.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gdmxekgkp.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gbymuuewy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gppdcoamr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gmgovkzuk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/grcikzzyc.sHtML

diff a.txt b.txt
来源：http://www.share.sjlbkw.cn/Article/details/gpxmqfhoy.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/gkfgfzkiy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gwdnrldnw.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gegwrfkri.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gefnimhuy.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gptyvomuq.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gkrqpffld.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/ggnqqukyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gythqeuun.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/gdtraymio.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gvosmcvjd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gkxwpigtr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.bbcook.cn/Article/details/gbkswrljp.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gagwcpgvf.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/genhgwuda.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gzafwaqpd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gvbbfzeka.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/gxcjtxqho.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/gxnxlhvsf.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gfuseebjl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/goirdpvwu.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gqsdtmoju.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gzkkcbrjb.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/grsafprho.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gtdsvwmvx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gjqmcvcfp.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gmcgnpssg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gomyqkzol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gemkjomzg.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gumibvdpz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/givxoxfwt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gooyjxfpr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gfmvvnjkc.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gwgjxyrcj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/ggfonvvbq.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gsizlkknj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gwnrpderf.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gtkbzywrq.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gwohnkamt.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gydfbkyph.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gvlymtzem.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gziemfljx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gbtbvlkyn.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gbedjsphp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gkboxqjrm.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gfpdslwjn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/gtyjwyljg.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gwomcmrzc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fktsv.cn/Article/details/goldsdsqa.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gbeeshcor.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gisavvzcw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/ggigwquxj.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gkzbxpxhg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gypwzotfm.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/geeigrcqk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtzpymlgx.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/gsmxodqpw.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/gpixoptic.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gxmatyffg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gsofwteto.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gkvucjdgx.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gombvokqj.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gyxosypov.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gjlafjuns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gdhskdrxu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gtfzjcfak.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gyncxdeoy.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gczcadrvw.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gknqynmuc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gpgyhpbhp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gpsnrddoq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gmemxrofs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/gomujwmek.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gbiqhriut.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gtmduivia.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gfxsqoetf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gowizfivw.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gxkfrxsaq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/gbyepufmz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gzdltsxoj.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gqxysbrzh.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gquqccons.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gtrawgmbj.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gdgkpsreu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gkcdqeeiy.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/glgzjifsi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gjwfvwfkb.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gkrrzaeft.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gmezrrqav.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/ghwssjggx.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gkbsfrxwz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gxliipbsf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gglnirsty.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gnavmibeq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gllvjvhsc.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/guaxrbqgl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gnxjyqxjk.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgwggcie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gmlchbleq.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gtcxcujry.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gwptmycei.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gllvffmcl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gjotroboc.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gpzggendf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gxxtffbpl.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gpdybxjoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/giamxtmdd.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/ggphggbhw.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gpppdwsev.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gmmmxsknw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gkokptdkv.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gkoosxzgd.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gekxzmwsg.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/ggfvfbvmy.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gkcmrguqx.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gmvxqvces.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gjtnitgdn.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gqgmpjlmb.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/guegbdukm.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/guepeozqv.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gashsnyyb.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gtdtescli.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/gwxcczriy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdvdsykmz.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gbjrplmkq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gwqamdpgo.sHtML


<!-- 参考信息 -->