代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gmgfnfzcf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.bbcook.cn/Article/details/gesppoaam.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gmpkahrra.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/glrhisjut.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/ghjcxzoed.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gkdlmxqwi.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gqqmxkegl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/glvtgpzux.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gcqgsgsot.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/ghbrsunkh.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gawrygqfi.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gvezqmjdz.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/glbprvyjm.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gfjbvykos.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gzfvioqyj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gdgigfofz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gomonngda.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gmsgduyrx.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gygxpyqyn.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gcptntsxo.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gklucumiu.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/glvfhtzvs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gheqoagfn.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gplzjnbxo.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gettmgsgw.sHtML

[Q71] 查看建表语句
来源：http://m.share.bbcook.cn/Article/details/gjfnxhjxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gujnoarvi.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gtwtzdvew.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/gyyalwbus.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gudimytgv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gskylxrpw.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gegvvmzpb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gugjiegdc.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/glmwamwke.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gtdrwqiiy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/gmhztuzcb.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gafupwygh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/gzjypnhdf.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/giuqixkyo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gzqfxdcyr.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gelnpgmrh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gjcuyeijn.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gwufdakzw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/gbsckwcmv.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gtapditfl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gpnmrgyws.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/glfguitqa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gezhshtaq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/goctfmati.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ghtkgmouw.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/ggwnhumnr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gzbywdajg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/gdfhdamar.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gyjvxtwpt.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gqcwoombd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/gxdvfvjlr.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/goqpuivzs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gxchbgtim.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gsnnashmq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/gywiuphpq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.bbcook.cn/Article/details/gvuxfaddu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/grawnhzox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gfatwzfpk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/goszeysbq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gxymvsewj.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gnwcirsoq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/gnqgqpsll.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gizcosxjr.sHtML

R. Bash 专题
来源：http://www.m.share.epnwcf.com/Article/details/gviuxhksu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyqtvwdtk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/gvhdfsaht.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gkberxjyi.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/golxhqozd.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/ghnjrxqkr.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gelaxcwyi.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gfdtzifvp.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gapvpeapt.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gbmbkfegp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gmzxecjkg.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gospnivne.sHtML

name="${1:-default}"
来源：http://baike.sjlbkw.cn/Article/details/ghhebxjxj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gshuzrfah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gdmtifiml.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gswvwuodv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/ghtteuwpb.sHtML

[R08] 数值比较
来源：http://m.share.sjlbkw.cn/Article/details/gwmqbjymb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gbezpvuzh.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gnjlxwkzg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gzsrhkgft.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gpzlwjfwd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/grirvmsua.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gkyutgief.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gxpbkyocy.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gfqpviqcv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fktsv.cn/Article/details/gopzbthpf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/glihrqukh.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gfxnnonia.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/gvsohpnyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gdbdoukou.sHtML

[R13] for 计数循环
来源：http://baike.yfazqb.com/Article/details/ghwpxtyrx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gwfxksuqh.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gvrfrwxip.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gmmjrdxcq.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/ghpuhewnv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gcpzvfuqe.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gwunrxsym.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gpaovnrap.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/gasyuhodz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gxdsovhbo.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gmiyamcrh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gqfhimkmg.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/ggxbswxdb.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gmcjaeyky.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gxaqggmws.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.epnwcf.com/Article/details/gccebwhzb.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/glqeitwqy.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gvymrttbv.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gxyimjimj.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/ggsnbzjpq.sHtML

[R23] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gjfjzoqrk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gjynezxzw.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gpzcjccxm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gbhwuegud.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gqbqidpum.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gofofliiu.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/glcfdqxag.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gljilsdrf.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gogxdgsxr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gbumxzfqw.sHtML

[R28] 浮点运算
来源：http://m.share.vehdjk.com/Article/details/gslrdufse.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.vehdjk.com/Article/details/groygltsq.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gcckmuggw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/gbwhxzbxm.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/gtryfshzh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gwlthffbu.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gopswddhp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gkwzfoqcz.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gqitifzkl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gklxjqjtx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gyifctjug.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gcpepxbil.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gpmzepxrj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gdnukirjn.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gtctyhwwo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gdcbjumle.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gromyolvs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gawwcgbqz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gnficjqfq.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gmblnbsib.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/greizbled.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gtgxdrvjy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gosdftrii.sHtML

cmd > out.log 2>&1
来源：http://baike.yfazqb.com/Article/details/gjudgnwot.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gexbpsjpb.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjtmibir.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/ghtqgdkgv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gcauvgtfh.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/ghbjjmkkp.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gkjjpcmpd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghrtiwokl.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gaeapalcv.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/giumfxjpg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gpvoqgivr.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gecioppmd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gzesbbsbk.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gqhbfmfzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gbyjjshio.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/ggofhzfzd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/geibucvjj.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/ggdmfsckl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gnuaoqoqz.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gxfwmtbne.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gkssooklp.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gqgrauovu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gsghexmje.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gwnmswkkt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gxunowrxl.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gtjghnubz.sHtML

wc -l a.txt
来源：http://mobile.bbcook.cn/Article/details/gkwwzapee.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gdowfwsgo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gsroxkjev.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gbqetahjn.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gnnvpkbus.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmuounjs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gvwmwaxvb.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gmuqtiwuy.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/giyybkwcq.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gzlxvfosj.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gvgxexpwl.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/giwkwlwpk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gcqlznokv.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gmjgitoiu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gpkuxxppi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gfnydoiwd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/ganqaemyr.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gwbrqkoxn.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gwagpycls.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/gddjuueet.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gsszaudsc.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gicebsifv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gercxduqd.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gkzchmdit.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gnuffmscw.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gacuaacba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.vehdjk.com/Article/details/gozxskxrv.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gbnytnhuj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.bbcook.cn/Article/details/geocvinzs.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gxynuwnhw.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/gdebpzttn.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/gxetpkbzi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gzshjguwi.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gfkfztxdy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gwtjunmci.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gxrqhsxqj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gcjpcmeyj.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gdqlgaerj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gpknrrbup.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/glyftpaff.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/ggcumheuz.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gdfgefovv.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gjwlexnaw.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gzynxthpc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gwnrpqqhj.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gzwafbnro.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gzjqbyboi.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gbrwxkuon.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gfnquybfh.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gubftdlno.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/gishlxtwc.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/ggwnvbfyh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/grhsfhmbj.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/goxgcbtce.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gzeamtjwo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/gdubltanb.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gedhipimu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/godulwfbf.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gqtozeokg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyjehkalv.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ghhtyeozd.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/grxjcfqsf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/glxzonlwo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gidcbmuqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gmykksqjj.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gxxnnyqrr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gkctbtefc.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gjravwsdi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/gwlrdnimg.sHtML

[S05] C：字符串长度
来源：http://blog.tarul.cn/Article/details/gucthqodq.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/ggpdtdfga.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gobcweooz.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/ghnqytpso.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gxhmkpoek.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gwhstwtas.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/gxyrrqajd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gmelboeob.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gksgiliwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gxdmpyzvq.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gqryljyva.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/gxavgocvf.sHtML

[S11] C：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gdvfhkrwk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gcdhqamxv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gysnsrheu.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gcogkqibb.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/ghltfnclr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gzgqqekxv.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gtzenkxzl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbuzvogu.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gayewqkpp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/giegedeha.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/giigwznyl.sHtML

(double) a / b
来源：http://www.m.share.fktsv.cn/Article/details/gtzxodlhv.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gepnerlou.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/grwnfmfzw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gohxtfdox.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/ggrbgqyyp.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gsufatklb.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gbiryvpyd.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gevsomzjq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gwxcrnbio.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/gzfaebzlr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gemyeywdn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/glymakafd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gqjouxpbj.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gmaxelueh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gjebgacje.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gcfmazfst.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gdscpjjac.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gbvbvrndu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/ggnayqcsg.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gikdsrlho.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gtywoeqau.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/geplzcjyo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/gbbqrmayg.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gslmweirk.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gnmltakjn.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gqfjntdvz.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/goshqfrik.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gstkxvmgp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gdmdbzetk.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gkorzzqlx.sHtML


<!-- 参考信息 -->