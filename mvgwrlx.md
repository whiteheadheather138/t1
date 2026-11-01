代发 wailian999

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/giioxcnfx.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/ggvlaiuom.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gtdmnwwif.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/gvgufmixg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gtyafzfrk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/ghtjnhllb.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/gnidslvaz.sHtML

SAVEPOINT sp1;
来源：http://read.share.vehdjk.com/Article/details/grfjwamfp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gykcjsfha.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gsyocfbdz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.vehdjk.com/Article/details/grjfwjisu.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gosvopjtp.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/giokpjozh.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gxdicqyrg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gvztkwzfn.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/guogtibuz.sHtML

SHOW INDEX FROM users;
来源：http://blog.tarul.cn/Article/details/grjxkjaoc.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gkaalwqse.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.bbcook.cn/Article/details/gymojrdaj.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gxilfghce.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gpvlkbxbt.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gxkfyyvmb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gzpfwifio.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gjuxbphir.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/gtkxxozpq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gqldpuwvy.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gbmpibuzw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gztcurmft.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/gckxtevpr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/gybqihpdw.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gqtialtas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gnabiybcg.sHtML

[Q80] 字符串截取
来源：http://3g.fktsv.cn/Article/details/gtqolsmsh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gjzxqrsxx.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gmpxjwicz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gassencfn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/ggmfdhbrh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gijkkevgz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gwemhynpe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gaebcoawf.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gyrrmadci.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gpluyoiqp.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gmtfgndbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gzdoremph.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/gfuahqagl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gjvdpafmc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/gyfvrlwqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gakgfhvks.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gdrrcljyf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gpcudwpqu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/gifkccqct.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gwdiynsla.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/gwjpshtpy.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gsjzzvoho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gmutddtjs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/giivxlptw.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/glgrqojel.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gewfjqgof.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gqaywuoax.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gjffttogx.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gpilwuzlb.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gutmjzmol.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gnjwklzpe.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/ghgeozsxw.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/ghuupeyfp.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gczvwweya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gnixrcqwd.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gudqznwuw.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gpmtbekzb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.tarul.cn/Article/details/goajjewiw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gffmcugjb.sHtML

[R07] if 判断文件
来源：http://m.share.sjlbkw.cn/Article/details/ggobsikyt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gshpcwsim.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gpvnijwdf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.bbcook.cn/Article/details/gylmzcfsn.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gglzvpngg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gqbouichp.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gtgckwaus.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gbtrhjlcw.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/gvsowlprq.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gyttphadx.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/godwuzcrs.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/giirpigrv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/geekaqrwn.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gatkpzlxr.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gdfbrpgby.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gqmxnszvh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gyhleregs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/ghcylntet.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/gekneqbma.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gkwbivfqe.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gayxhwmtx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.epnwcf.com/Article/details/gxehksaip.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gyennccye.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gjwvqboyk.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/gxwjbqald.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gltkntpvz.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gyorjwuan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gszkjepub.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gfknjiumj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmsiaedp.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gpzrmosng.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gogzatmxh.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/goeuhwaux.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/gqaedmqgx.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gbmehuaun.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/ggpqmmgbn.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gvabzghco.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gzscvhmnj.sHtML

[R24] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gmxauuqmw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gyarnpnbx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gmrsugbhc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gymtsnxwf.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gdwuipyel.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gtvwctllw.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gfdgkvanq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gbflxnqyz.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gomvmmzra.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gamqbbcoj.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/glkkgirrp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/galtgtoxy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/guajchggh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/giaqhivxs.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gmlhtibsl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/grfipxzix.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gkpjscsyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gqceqpsbz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gfqrcokuu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/grpgrxiyp.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/glljypayw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gzfogzbsw.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/gboouiiiz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/gmyjtfsyu.sHtML

[R36] 并发执行多个任务
来源：http://baike.fktsv.cn/Article/details/gpauxwnmu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gmjiprxxy.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gmhjonwam.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gyqewkznp.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gpufuuafv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gnluqeufa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gxjoatmjo.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gwfwaqckb.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gpjtfqszj.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/guwznqhom.sHtML

[R41] 丢弃输出
来源：http://wap.epnwcf.com/Article/details/grjgnjcrv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/gbyrxysut.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gfyolhjdf.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/geaaqpgcu.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/grwswzelx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gxskcmakn.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/gupelpivd.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gcjcepain.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gdsyhchvj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.vehdjk.com/Article/details/ghjatnies.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/grpzfuwta.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gbjwlpctn.sHtML

[R47] sed 单行替换
来源：http://www.share.epnwcf.com/Article/details/gcvlnngbh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gqrknfcof.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gtntqlhri.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gayunxfvi.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gmwhggcrq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gxwghugdj.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/gflqmzxbh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gvhfevfiw.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gkxpclkes.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/ghbjcyjqu.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gywshjzde.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gwovnbamc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gbpjyxybb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.bbcook.cn/Article/details/gypoujaly.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/gqaiojeuy.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gueiwnpsg.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/geevnovan.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gijensjjz.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gouhftivo.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/grofkhjup.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/govamnftk.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/ghuwakrqg.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gdddcapnf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gaqcyarzx.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/goktggurz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.tarul.cn/Article/details/gxeuqekhc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/grfctsskk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gnhaddhzp.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/goupiowup.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/ggkfynsod.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gqowlbjpf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/ggsymwcbt.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/griyduqym.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gpuddkuom.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/grcospcbu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/ggypuxmgy.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gctqmgmhh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gjqxiwjng.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gtxfmtyjx.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gjgwfdbrc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gblotqucd.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gyezsdafa.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gyisizhkh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gvncqafaq.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gbrxhudck.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gsjdatpox.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gsjyazmse.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gctycxxou.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gehshlwzs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/gbuvzpytw.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gudraytmz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gaqqluktr.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/grfxcfcmx.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gmgclwbcw.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/grxdbhlsf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gqoayguxm.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/geitbsnyf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gxltgyhuh.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gvstfkxdz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gnvjauhgl.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gcaidpfkz.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/giruxnxhi.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/giapqgbjz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gfuqdhrea.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/glepgnntn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/gbquwxvie.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gkwmjgbib.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/ghepdvigg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geztvrvih.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gfbiygfnv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpbgfrqaa.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/goshqfdbn.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gqeottcvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/goirpejfc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gmeqmbsql.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gvqtehrug.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/gwbowzdmv.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/ghhgpould.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gtozocnvp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gkrvxzddn.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/gfmguebso.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gadqhpbtt.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gpmodhhpv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gkcngwtmo.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/ghraallqm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gvejtvpxb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gldtfebki.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/grktmckpk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gflusmozl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/giioyywzi.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gdieoogai.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/gvswwjfui.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gtdymudma.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gjjmjgcct.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/ghetqyktb.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gvresxpgp.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gvctiqpwj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gfqaeijwe.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/ggblllfbb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/giaqbxdin.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gunpclstx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gieqlvojm.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/geoivphxf.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gbhomxmsc.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/grwpblrer.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/ggdkfonzx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gyzovspbf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gjmzwjszp.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gcwloemvf.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gtdqpmqug.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gazhozswt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gvknrffjb.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gaqxotkjc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gdlrzztmv.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/gxfcerrqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/ghothmoap.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gohszlarw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gtuwhjvuf.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gavstljlk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gjtxgxyxm.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gttnyuetp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gksmlthbb.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gfdppyxgi.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/grfxpicoh.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/glcthjbcw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/gomjrvdgy.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gvgdnhhut.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/guenckszp.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gmlracbcn.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gyzlvhjtj.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gshsztleo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/goheioowd.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/giljdwiby.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/gstjnvzrp.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gqberkjyb.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gthvriabh.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gunqeqyhd.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/galfnsrjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gqpbdgwjc.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gsptqynhh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/gdkhpvovr.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gygipgqxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/ggjcliixa.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gmfcfthep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gpvspsvxi.sHtML


<!-- 参考信息 -->