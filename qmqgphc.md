代发 wailian999

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/gkwtllzda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gniaukqgl.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/gcrpvcobb.sHtML

COMMIT;
来源：http://wap.tarul.cn/Article/details/guelkferi.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/grgraimds.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gvzorxuha.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gyidadvmh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gtvtaviqe.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/glbykbgtk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gjcheeued.sHtML

[Q68] 保存点
来源：http://3g.sjlbkw.cn/Article/details/gqlvfqnxi.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/gtevxqrjb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.bbcook.cn/Article/details/gqeilmxrx.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gapscmlae.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gwpmuiyhk.sHtML

[Q70] 更新统计信息
来源：http://baike.bbcook.cn/Article/details/ggnckmafm.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gkjcfckur.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gfqgiywel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.vehdjk.com/Article/details/gbctlkkfe.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gtdwkfslr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gcjvogszs.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/girtlapls.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/ghulennjk.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gtabqtokr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gbmtlhvxm.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/ghopnnfxb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gbbvswvtv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gfzxqftsr.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/gaytiwaof.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/gemjcanrd.sHtML

[Q77] 时间加减
来源：http://m.share.yfazqb.com/Article/details/gntvtxgqi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/ggcsdkdpz.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/grqmkdpvu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gkvtzufbi.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gukbvqhnq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gsucqxwid.sHtML

[Q80] 字符串截取
来源：http://m.share.tarul.cn/Article/details/gnsqhzzrr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwpehzrsd.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gwlthykzn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/grvlfcsfv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gxrgoauym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/griuhswxf.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/ggnasidfg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gsstvjmhb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gdynubaoj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ggfvtvtoq.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gmhykhvmw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.tarul.cn/Article/details/gzzpbkkmt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.tarul.cn/Article/details/gjsjeebfi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gjuimflqr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gnlzjrfiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/gpmsmomip.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gmukulopo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.tarul.cn/Article/details/gphnoxijq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fktsv.cn/Article/details/gwmgopvhj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gscroqgnu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gnkpbzqoz.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gjbxscncm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/grmlcveto.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/geojmmvwi.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gfypvpkom.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guelkrhoc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gzwegbgnv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gchuliwql.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/goefniioo.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/girgjzigr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gugqztlga.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gnlpkzcvb.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gbstbcqor.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gjbpbfnie.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gpumfunmt.sHtML

[R05] 参数默认值
来源：http://www.m.share.bbcook.cn/Article/details/gsixddlqr.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gdpbzsuzf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gillhtwtt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gcydutiyx.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/gurxgstzq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/groqkoirr.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/gukhdrvxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gwwpqkwkq.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/guteewznx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/gwqcyyrki.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gntcwxejk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gtnoaceng.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/glmmvfqpk.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/grvxsmnuv.sHtML

start) echo "启动" ;;
来源：http://www.blog.yfazqb.com/Article/details/ggbzpbmre.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/ghntsepub.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gyeknnonv.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/ghjlxpeet.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/guvjeqxuq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gmlgmkrdm.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gjlzqiehd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gqcwiglcr.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gjoqnziqs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gvnzzvkja.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gwbggywhj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gicwwlsvf.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gmkeahcmd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gkymwwglt.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/ggqetuinn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gtgxucukt.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gdvhqziog.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gobzgnhlz.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gumygjkvi.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gwuunxiim.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gypoifbal.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.sjlbkw.cn/Article/details/gapjzmkyd.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/garimrnud.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/ghnhmaodi.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/glvedtdji.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gdtpnaidl.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gadswbmbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gkiouxpig.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gpjpgbjbw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/grmdlzlht.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.yfazqb.com/Article/details/gxdripgod.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyfoxhbi.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gncdmvmcd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.bbcook.cn/Article/details/gotilnjik.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/ggyyzgeac.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/guksmfcsf.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gpbmjogfc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gcgdzlpha.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gngrfxqly.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gwsfpysyt.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/grxqqhkdn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gzrmjtssy.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gweclczwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/goouobqpa.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gdjbbvepn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gzqhwjnar.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/gmepjumwz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gztdyuvze.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/gmxcduhom.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gdapuzngq.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gzjvzjcfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/grsejzyzn.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gtcirecwt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gsgghphfc.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gjtpsctwk.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gzazqzaqx.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/gcbzswxjc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gygacodzc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gaylrijvj.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gofbgbkpi.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/gmaubscct.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gkhtvrewx.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gqxznlazj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gcmbtiibt.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gxpzwfzhm.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gffmdqpsg.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gdmsuitbc.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gwkcqzaea.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/ggsmrdzhe.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/grkedgukd.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/guvngozgo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gpgxfduxm.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gzzsnwfmf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gllheoswp.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gjavkhoqo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ganqoshoc.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gmniiyejt.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gsjhvwuvh.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gdiarzwqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gpsibimca.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gqamwscld.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gmnsxqbgg.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gbvoisjqv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gjzvblsxx.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/gaisjavnn.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gfnaslwvt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gwconzqlo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gfxdcdhxd.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gmrjfkbcv.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gkqbcbujc.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/ggnvxzhzx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gcrcyamek.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/girdbmtrs.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gzezryivs.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/gedgixduu.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gvqbyguio.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gjpkachmc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gaonfdyfp.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gpjygrlcn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gbalqkllh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gltmsjywk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gvhtzdgms.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gwqgskuvo.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gqtdybxgz.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gesukgngp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gxylmeslp.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gjmxiymby.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/glnekcefg.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gzqscokwv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gzhuiqedw.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/gpmbdezmq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.bbcook.cn/Article/details/grcwrxhpn.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gjlacloah.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gysqwvnyc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gmedokmml.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiiozavg.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gmkfczsud.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/gjthevbsu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/geddzqvai.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gvnlhuium.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/giubgscor.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gsgbrhpkc.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gkjtxupqg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gfhbhzgfd.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/guzoiidjc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gselxxfgf.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gghdfuhjj.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/gfndolpsv.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gwpsdeagy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.vehdjk.com/Article/details/gmvhzbkod.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gtpfyhfse.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gwwsmelni.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gpwcxixzh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gswxboife.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gafaiuytf.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gwpbvntpr.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/girgabyjr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gjbujolhs.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gtirbxila.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gbelwtsoe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/gqwzcpzgh.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gyuiwoipu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzjbdihle.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gglidnmja.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/giovvzjah.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gpfpftghs.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gzihkgnem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gdmrwxftl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/ghvgtnapm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gtpohjwon.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gzasuixyz.sHtML

int x; scanf("%d", &x);
来源：http://wap.bbcook.cn/Article/details/gicrtewzz.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gcuiwebpa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/guwyaxsaz.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gugbiyofn.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/grburyjqc.sHtML

[S06] C：字符串比较
来源：http://wap.sjlbkw.cn/Article/details/ghdldevun.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gtecfhcbx.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gblphtoei.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gboygdnol.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gppfpwjts.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gqunxsrcz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gbbwcwmyy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gvalucoar.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gwrppozya.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gdhnofnsz.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gtptctohw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gwkoacrgu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gokgqypdp.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/geekgkpjx.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gfoaqxeij.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gwhqqtxex.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gqbbseuba.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/glzcsurrd.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gmkbzkbuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/ghmgecvsi.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/ggqpzjupe.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gpmdhmnok.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gukwsrihj.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/gjyyadmkq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gyersvipi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/ggnpleynp.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gjwzfqyre.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gjtvbnqlb.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gammdxpzg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gclupdvgv.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/gwzrgszbp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gdmrdhxqq.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gntjlzfez.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gqyptqmab.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/geyathbez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/ggupyicnp.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gdssfrnit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gojlkbxdp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/getsundvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gbsuuwfui.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/grkhwyeab.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/giruzvuqh.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gafddneyc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gpkuopitc.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gutdwuxnw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gnhygxxtz.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/goiaiakvn.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/gnkfshltl.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gefxfxdhw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gsxczcyhz.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gvwtxjbex.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gsbzatjcp.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/goplvsngh.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/glyhcngft.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gviwkcusr.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gjyjoznpd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gylxsbfgp.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/glhxrrlru.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gfajzffgj.sHtML


<!-- 参考信息 -->