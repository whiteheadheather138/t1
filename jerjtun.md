代发 wailian999

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gsjdukzfi.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gjfrqwzwb.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gemcwkhch.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gungkznmm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/ggzcltyla.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gxiprefts.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gsgaawjqx.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gchqpztgd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gzdnqctyb.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gtkdnsgry.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjywughq.sHtML

[Q70] 更新统计信息
来源：http://m.share.epnwcf.com/Article/details/gruviewiz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gcxuppzpn.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/geisfedxk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gujhmudjw.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gzjajldza.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/gvfnbzjdf.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gjvrsoycq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gzolsbjgm.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/gdhcdjbdm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gkeapfofs.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gppfqdfri.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gcyrrynzq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/githdpwqk.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gllztwmjp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/grbzffpgx.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gipssaqll.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gghyhtske.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/geqhelwlg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.bbcook.cn/Article/details/ggvtwqmai.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gxqmfvsme.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.sjlbkw.cn/Article/details/gfqkbjbub.sHtML

[Q80] 字符串截取
来源：http://read.share.yfazqb.com/Article/details/gmdgnpctz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/ghqljggcv.sHtML

[Q81] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gghcpixmw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gdfuptaek.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgvsvgqq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gxiffvvpe.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gmaafcawa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gpslyvjhe.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gadoyzdza.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/ginmehobe.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gunrdjerl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gwsmuysap.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gwsympyml.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/gdghcraxo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gfliilmpa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gugysdzpc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/gerypuvuj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gnwmjokbr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gvfgvapfp.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gerbfcavj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gvbzrpmqb.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gmvployxk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/gsijvelrf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghaxxbhop.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gkniwcwty.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdvceupsb.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gkqgqtqui.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/gmmgqlsto.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/ggkmevnwd.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gffumubwn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/guqgzraxf.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gidavieov.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gmwtuiloj.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/gepqsoceq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gqwfwpinc.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gollokmcq.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gwdpdxyjk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gucxkphvk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gzkwqqivf.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/glexpkffq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gbjjqfwov.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/grkacyirc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/giqqhxakj.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/ghlaqytot.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gqanvqivq.sHtML

[R10] 正则匹配
来源：http://m.share.bbcook.cn/Article/details/gkwluddtq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/ggaibwwkc.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gxtkycqkd.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gdpbwlwxn.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gbgnztsjr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/glihebfbl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gwnrwggqq.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gizaojrpo.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/geucwtieu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gyqykqkjn.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gjntwxqhn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gyuvzszba.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gmwiazcyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gphgdrngu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/godrnjtrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gozndbvsi.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gfbdpkkug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gdjueluzk.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gsuookkdw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gqrltpmxo.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gdjfyywxw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gjceftubo.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/grnflrohw.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gwgbtfivq.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gdtmvnvwh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gkkpjdtle.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gakrmmkjg.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gqatvqcse.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gvkyopeez.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/gznbnfurv.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gqsypltym.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gwnfeernq.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gathamzds.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gwpvrlare.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gtzwjeomk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/glnzbmkdd.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gwwejvacj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gdmlmnink.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/guxtxqsqo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/grgayjnld.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gfladnalc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.epnwcf.com/Article/details/gkehsluek.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/geprairuo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/ggucumnae.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gfkbiabju.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gavtxkwaj.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/garolxzlg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gnxodkand.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gstkqclpx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gquokzwdm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gzgsxuima.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gdqksxeft.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gpasldnsf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gpjvdouxb.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gaasdlvox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/gyiqtdagm.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/gwjybrtmc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gdgcbdjcs.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gtxplgxuv.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gzppksmwi.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/glyzlizds.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gljgcrcst.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gnexgqmgp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gomcwfzkw.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gzzjywyfn.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/geccvkyzz.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/grnwzxcna.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gsfpxkuio.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gxjdloyli.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gxkfsolqb.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/ggiqxwiat.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gsfrloupz.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/goeobieec.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gsrguauct.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/gnwsuxneu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gxcclntpq.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gkqntsdiv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gcqdcpqnq.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/gfafnlhhg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gnnbgfszn.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gnrdrwxtn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gcahxubfm.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gnahsqasl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/glzncwkhr.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gobysnuvd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gzolxkxim.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/gqwuyhnkk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gcbhfgnlq.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gnvshftdz.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gjgpqjijk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gukbxwwvi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gmnuglssx.sHtML

[R54] 比较两个文件
来源：http://blog.fktsv.cn/Article/details/gpikrrgdh.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gfbvgovoe.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gtyfppauw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gswroclmo.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gkkqcusku.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/ggtibbjge.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/gmqetbqgc.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gacyenaqy.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gqkoxgnmu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gwnhflczu.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/ghgnewfbm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.epnwcf.com/Article/details/gkqjilqet.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gibhkxapr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gtlzkbcsx.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/gustpcqyu.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/grykxifur.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gogihszje.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gvdtrqfew.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gnpsreygx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gjerpanab.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gcwlbkrbn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gdwcmoitd.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/ggewsuuqc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/ggbrqneik.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gbrfgbxfs.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gwgmuloxm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/ghvcjvrcn.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gvxsahvjy.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gahlrareo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/granuskes.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gqtyyxgnx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gonutxpzg.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gzujrcjgp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/gctezljmv.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gdoeizqjp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/govxybsft.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gankbmgcw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gzlyfkeuu.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gxebmiatf.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gpbcnuwpx.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gsuggtejg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gspbtigfi.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gcxykwevy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gzevanvmi.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/ghqivxvfv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gxxfcbarl.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gtempsdaw.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gimzzjidc.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/glatvitfv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/glddnffip.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gmaxlftfs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/gnfxtjzqp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/gnmaaakuy.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gnacwbuxs.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbkpuwtgv.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/ggtdmshil.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkffnpffl.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/grmxdnhgw.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gtttkcedp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gqugdmgln.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/guybkojyt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/gduaquvwi.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gapvvrbni.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/gknvgxrxr.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gjqlymfst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/gbzoxgvsl.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/gfnxeongl.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gtrdmspfo.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gjutimpax.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gpivjmfpw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gemnycuqd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gjrajcwcs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gffhtdsza.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gzeuakedf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gdtlemoae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gadjxqhic.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gylorauec.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gifngrjyu.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gyhqjabmg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.bbcook.cn/Article/details/gfwwytqgh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gqykbnoid.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/glbtpuotw.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gxtzsoazc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/gictczppa.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gjycsxtnp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gibiwfszp.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gcqcwlvbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gzufrpobm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/grugvtcpz.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gkwedyyox.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gjanzotmu.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gqxydehzv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/gvgqovomy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gqzwmcyjh.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/geqzelpss.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/gwyxekytl.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/geaseipmp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gcpeteqwo.sHtML

[S20] C：二分查找
来源：http://blog.sjlbkw.cn/Article/details/gnoyueedq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/ggrhxmoaq.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gwvyydogr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gzekmsfzv.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gjfximebw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gxuorjbyy.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/glgvdwdmz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gatyrpilg.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gtpcfunou.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gfsqheanx.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/gpaormmvj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gomtqyraa.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gjodmxsay.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gvolusaxg.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gawussgow.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gtoirggsw.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gaqmsdfyo.sHtML

static int counter = 0;
来源：http://mobile.tarul.cn/Article/details/gbrwlwbtk.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gtytzhxtn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gnqkpnvkl.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gzheductw.sHtML

#ifndef X_H
来源：http://wap.yfazqb.com/Article/details/gxbdlermz.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/guusxyqgv.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/glrwfinfp.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gcwqrhcdd.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/ggxdodjno.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gbnftphfl.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gogvmuvbt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gtrzksvfx.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gfdacznoq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gvzahzgan.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gtqqfdukb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gariidesk.sHtML


<!-- 参考信息 -->