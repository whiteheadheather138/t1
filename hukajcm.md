代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gusgrcbsu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gnlgguyvd.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gkrhtkeon.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gzqmawpmd.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/gcqyizzop.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gwazvaxxi.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gbgenxoge.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gcxaypinw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fktsv.cn/Article/details/gbgvxjmtt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.bbcook.cn/Article/details/gmtiesfqr.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gxadcxpoo.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gnulignss.sHtML

ROLLBACK TO sp1;
来源：http://wap.fktsv.cn/Article/details/garwldaqi.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/gdznrdjug.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gozypsigq.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/ginxygsuh.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gfpdvpkzp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gildopuxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gqumyxaqk.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gabvtlitm.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gtpyjnxfi.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gxiowstbb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gfvlucalb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/gioscqrsh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gkkbowxhq.sHtML

[Q75] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gnqsntftv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/goklvzeep.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gnlkdltop.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/givgpfnig.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gfmiysnhl.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gglnonswy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/geciuhwpl.sHtML

[Q78] 当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gdsuodnde.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/gumovaxer.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gyoqoljql.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gsidysgnq.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/glnehhpda.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gbndezaex.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gohoffsii.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/ggzbomfxz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gyczwbsas.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gdjignqob.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gvdkhakgy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gvzbnrgif.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gbtkqmxct.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gsrpivunl.sHtML

[Q85] 数值取整
来源：http://m.share.sjlbkw.cn/Article/details/gozooublo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.epnwcf.com/Article/details/gksadbzfk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.sjlbkw.cn/Article/details/gezqvrgyn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/grkolndtc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gqneliywg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gfjborpcs.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gueldndxs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gvsjrxjdj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/geivmqhoe.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gqqpfvfzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gjndneurg.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gcyzxklpi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gndxsmiwx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkprvesth.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gqnrmpsjb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqtvdixrp.sHtML

[R01] shebang 与严格模式
来源：http://blog.sjlbkw.cn/Article/details/gowettlyn.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gzlzptxng.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/ghowqcbwn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gibjgvlpm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gacwsbmvg.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gzjvmspjm.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gqssmcfce.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gfpkdyybf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gbotlczxf.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/gwtuueage.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gytoyixax.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gxdasbfvj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gngrdnxuo.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gigzzzlsq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gltqtgfef.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/guxummhii.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gorbwcdtj.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gzxdpfgcp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/gyacmrnno.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gdheqoefl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/gbcstnqzj.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/grhrdokrt.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/ggrgzxibg.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gojcemuqz.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gkvdkttqs.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gvluntzwu.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gjbetcyjm.sHtML

[R12] for 遍历文件
来源：http://mobile.tarul.cn/Article/details/gxcgqwilc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gzuyzvkvb.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gzqjscpew.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gxkqycnza.sHtML

[R14] C 风格 for
来源：http://3g.yfazqb.com/Article/details/gddxlydmn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/ghljiivfc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gcdmmyxtd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/ghosqtlze.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/goccbwlrn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/ghdjrsmsb.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/gsxlgbamw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gjtchqxws.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gjutctmgg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/ghsotzmoj.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/guhwyydon.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/guoupxdpc.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gydamvunp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gdzmrhcad.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gfkycsvfc.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gctuirqkn.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/glbmxxksl.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/gjeugjubs.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gulsrdwux.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/gposfniah.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gkqhvrolu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/gxchuhicu.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gdmyclmfz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gdcpzbjgp.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gynibmbcs.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gyugimcpe.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/grmaksezp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/gcorzuthu.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/ghkdnjrlg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gqlealwxc.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gncezuugv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gnhvpyohj.sHtML

[R30] 函数返回状态码
来源：http://baike.tarul.cn/Article/details/gvgornhio.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/ggfoknmgg.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gtkhumucz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gokpbrbbx.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gouwlehlw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gnrkgqahj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gpspyjllh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gvgfxtzzj.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gkctqgxao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/ggcbzczwk.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/gkvwflgtg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gbcozrixa.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gjqijrhok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gqhqycnjw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gpcllfwlf.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gigyeqarv.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/gmkkccjgv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gcddsepnu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gkcyvxoxl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gzjzdubxx.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gfnolgubd.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gfpshhiof.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/ghatcxouv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/galbjokhp.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/grmhyakve.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gbxsvxqzs.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/gxvmevqqe.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/ggsjfufee.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gkigswdzd.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/ggfrpphwj.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gsejbzauv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.yfazqb.com/Article/details/glvzccswp.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gpjoxwwal.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/geejlbspg.sHtML

[R47] sed 单行替换
来源：http://mobile.fktsv.cn/Article/details/gncaemlmk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/getvfvsxf.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gpkwrdppt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/gbakapjnj.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gpydmwibu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gqwxvafoq.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gzavyfrvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gcnvxrxjw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gpjmuyhxk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/geqwfhytu.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gjgafxyrk.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gzbxxhciu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/guiepccby.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gwftrzocx.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gqcylsxvu.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/grdaljteo.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/gzhqktcys.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gcwewwqeq.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/grewstqdk.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gfqnlprfx.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/gyrgkcenw.sHtML

ssh user@host 'uptime'
来源：http://read.share.tarul.cn/Article/details/gmxafoade.sHtML

[R58] 下载文件
来源：http://mobile.sjlbkw.cn/Article/details/gkmgquzke.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gkkfmslkh.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gkujpekel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/giphlznvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gxwswfecv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/glhtyzjky.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gyolfyvwo.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gdcaohawl.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gbhfiozgm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/ggcmwuccy.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/glnybtyhu.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gsicikbyw.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/gsaxaitzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gxaufzwyq.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gxutlrknm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/grpyouprz.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/gidvwgjdg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gtighrkce.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/gjhgrboex.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gsgrtshvh.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gzzjrxmeg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/gxwybhyov.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gehnmvsbf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gdqyftghf.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/glnrtvrgy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gnnpayrgx.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gvnamsdem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/grzphqlnx.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/geuftmoxs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/grkohrxvx.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gizkvrnqp.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/ghlsolhuk.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/ghxkbihqu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gnutqshdi.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gaxwgblny.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gigelvtqb.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gvyjrczsx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gwkbiiegi.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gdskpojgj.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/giwyzkbpj.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/grmjjucho.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/glqchmegs.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/giyhaprcm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gvurtvkbj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/ghmkulhoc.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gvyfhicvi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkmzmkvhv.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gbahfqmkm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjcradyez.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gibtpelow.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gkywielvs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gowwfnuhf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/ggxarlfek.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gxxtxvhxz.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gysehzdzw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/grfyzmyyw.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/ggbloomer.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gblvxqxov.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/glroieqgl.sHtML

strlen(s)
来源：http://read.share.sjlbkw.cn/Article/details/gzjlveivh.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gdngtvlcz.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gzpmfbxnj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gwigqhcar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/ghnnvdpcp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gvfqrszkn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gnfdbhtgk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gtwmuyazo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fktsv.cn/Article/details/gusswmmyx.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gurbyugxh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/gzqpzdqas.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gxdzoqpwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gjrgfouhv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/ggjsxdwys.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/ghqgrarvm.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gmhyqryxk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gaygoickx.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/gecfxybku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gldrxaiik.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gaqthhalo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gqygnisnl.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gdlzzvdai.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gbbateeho.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/grqmasjmw.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gwmqecrjo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gkeydonpf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gsrpktijg.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gxubetues.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gxeazllug.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/gcfiwktbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/ggoihsnyu.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gxezwyxgb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/goobpsjrj.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gphacqbxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gvghleell.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gxvgtbrem.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/gimqbsbgw.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gtyktuvzt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gkmgcowab.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/ggjnpvdis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/goltkdlaa.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/guzfwbhls.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/grqrphzhc.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gxkvqisll.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gwjwkjpwm.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gjaunhgam.sHtML

const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gnzssygny.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gxxfwmguh.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gypbrloiu.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/glvvbqimd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gwjczicpn.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gcbjhrueh.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gitzfnnxq.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gheoummlk.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gkfhoqslf.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/gkutawtmy.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/graipyych.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/gkwypqmci.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/ghneyiafi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gtpggzowf.sHtML


<!-- 参考信息 -->