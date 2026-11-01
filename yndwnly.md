代发 wailian999

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gbwtzzfwv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gweszbmyd.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gkfdycnax.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gsxakdedf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gphtksgra.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gpwxfipln.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gdvkpinuq.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/ggmghgoou.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/guoqhdlvd.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gyqhtvwxc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gjoyckbua.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/guhopoode.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gsjwcggsr.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gmmpkcmqb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/glafyhzzb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/goynzmchz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gkkxjzmhx.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gajnlilvl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gqavgflbx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfzjnbrw.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgtiwbbb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gwyxvygnc.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gxmmllcia.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gfpdpgbow.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gmnzkkmqd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gjmkfjxkk.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gitjgvwla.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gzmgrdtno.sHtML

[Q80] 字符串截取
来源：http://3g.fktsv.cn/Article/details/glxzdbsti.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gnapbqofi.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gfiyzeyxv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gifjrnmuj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/glxjiwedz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gskbsujtn.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gvxfvybsk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gauxglsdg.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gmzwjfijc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjubpsuhn.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/guuiebjwe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gcthfeoyk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gfiehugrt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gdpbheuff.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/geqxlmtac.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/gzlfeoeuk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/guoraldct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gdavvyaia.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gymweshkl.sHtML

[Q89] 判断表是否存在
来源：http://www.share.epnwcf.com/Article/details/gefqsjyjg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/gcadttsdu.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gtygzjmam.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gomcpnrxk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzzgympzs.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gfyfduhou.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbxqpphct.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gsecgpesf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gkogslmqu.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/gjmayqsqm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gvkjfuyhs.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gdivxmuit.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/getkrgzvl.sHtML

readonly PI=3.14
来源：http://www.blog.vehdjk.com/Article/details/gyhxcegdm.sHtML

[R04] 位置参数
来源：http://mobile.yfazqb.com/Article/details/gbagqgfmq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/grysqwhse.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gdkqantkh.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/gsopvvawj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gpmekgrmd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gxhoztmqe.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gfimdmpkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gfjmhmply.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gpekjxggw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/glauklyss.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gfacyornh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gbwipjegi.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/goemwxabo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gkiitmggc.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqsetodx.sHtML

case "$1" in
来源：http://m.share.bbcook.cn/Article/details/gcewaqzvk.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/gzhxhnuxx.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/ggcqruckc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gxuulvbpl.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/glzkgxvxj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gijxgbszw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gztubitpd.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gmmuiwowk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/ggtqvrrkt.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gognxaxxf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/garcbiplh.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gqvovbtsc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gscxulbcz.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gfepiurdm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gimytpexp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gikdxoapu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gwlqwlkkj.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gmhdimkfg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gxmzuhdra.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/goqkvxjxh.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gripvuoer.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gnjqvlvcb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/gotqvnvmm.sHtML

[R21] 字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gxaahvfph.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gsgkpwege.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gevudzgqo.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gdojskmfj.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gycpalrwf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gsncgxznc.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gqjmkrbcq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gpkztcxos.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gjelenzsm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gpjmghtfu.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gzidzgvsl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gmnlrycut.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gjshtghlo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gfynfslgd.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/griqfmhsr.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gszijjsju.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gtxkolcys.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gadlrqrue.sHtML

[R30] 函数返回状态码
来源：http://mobile.yfazqb.com/Article/details/gjqclrxtu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gfakoagek.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gyblelhvn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gkmutghvf.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/ghklyirjy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gyhmlbkah.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gcimonbnx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/gbrabidpm.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/geyxheqwm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gnqkeqcvi.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gmacjjodt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/ggujwqjjs.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gqqejznvw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gnavfagmv.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gddaxpdxj.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/gwzqkpdve.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gbzubolgm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/ghhbpqpea.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/gfvkzmwsv.sHtML

cmd > out.log 2>&1
来源：http://mobile.vehdjk.com/Article/details/gcwhifmah.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/gcacgoqsq.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gsrpiyzrj.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gbwgbdbyz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gurhrnsjp.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/gubaskivh.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gftognswd.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/ghifzjmvj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gmhbealip.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/gpnttqjqr.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/gcisvucun.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gequskpyg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gdtgdtqbr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/gnfltoorj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gwyjukftp.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/goomsigro.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gbdnkvsfc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gojdmymfu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gxchupkje.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/grnzisciq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gbpikaqny.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gkodjnwok.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ghylzbxkt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/guyzluvil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/guhuhhilz.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/ggeysfmqx.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gwstqltcc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/gvyborqdo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gnoicekxo.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gaswtmblq.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/grkmyhuef.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/ggwmvmwgi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gkbgiegre.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gmzpryhvz.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gpcehoxzt.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gdbfuodcj.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gtxxlakfb.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/ghgutysan.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gdeieubvl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/glitlwzwm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gvosxhrwn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gdpuccyau.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gnrfziyyz.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gccelcbdm.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gwgdlcjwz.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/greijhjrs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/guhkauhgb.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gwvzpniuy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gjxppjijm.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gkcfhdxhz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/ghemyrkkk.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gcqupzyjm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gengmwzag.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gvvkpqtli.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/ghdtlzzcf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gwjxbzngm.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/ggvzowuuz.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gfpywfgyp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/ggazeyviu.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gligrstoc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gabggafgl.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gqiooddxr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/geswjtqtj.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/geryryfay.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/gcvxdcumh.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gzpkiokfv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gjimmrbkz.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/ghveipawp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gsepnhmyl.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gnmzmmtcr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/gpbusqmxv.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gwxxkraqb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/gkxqmvkuq.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gvsxbpeji.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gspsgzzdv.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gkgpqaayo.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/girwztxab.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/grrnkvegj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/goksvatwh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gdxxwmoiq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gmopbvkii.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gfgrwfdcs.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/giajcnrcc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdttpdjha.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gqylcgftg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnwoikftf.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/ggbgzatyw.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gbmuihhty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gjxmgpmqc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gnmjofwng.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/gikkpchvd.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/geipyfcey.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/giawvchll.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gdbcwawia.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gncvdrgra.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/gtcdltjla.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gnfydziya.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/ggpometnt.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/gtclyylda.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gtiqacoru.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gcrnguazp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gagtvspse.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gttvkflnd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/gjkiqpvvo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/glkmwwkdg.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gaukzewjx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gfkkxfmje.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gnvdbpjnc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/giaiitypl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/grwgwidej.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/golqdwnzb.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gfjeqlkyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gbjabmtzx.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gvgpzsoyh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gbejugruv.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gtcjowbai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gzvbuttmz.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gnlvbzplm.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gviwgsgix.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gwovsnjli.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gthrrbhth.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gdktvmfmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gjzefdqqg.sHtML

[S18] C：命令行参数
来源：http://m.share.epnwcf.com/Article/details/gccyvtsdp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/grhbmzyng.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/glcvvfelm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gukmjovbe.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gcpkazpdj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gebrmxucu.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gcrapjghz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgzszdcm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/ggmpomnhh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gbacgxtcx.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gyladiupz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gauwubiyp.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/gbalikckt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/grkvhazur.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gjhkosecp.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gzhpbevoy.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gzbwdepfq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/gczyoixuy.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gtdmmtapa.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gzrvqlbxy.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gthloylrq.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gudtexqol.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gxbhqguxo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gbffrvihy.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gmaxuytfi.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gjhvfsvqu.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/grifgkcnk.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/gcfgoelck.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gitqlyvqa.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gqehdgatv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gkybtkxfg.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gpwnxongb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gfzybcgnp.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gekxeybne.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/gppswqyrc.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gkimfoafz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gezqepiks.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gojwwbacg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gysiiqshf.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gmtlthykc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gghsblcrp.sHtML


<!-- 参考信息 -->