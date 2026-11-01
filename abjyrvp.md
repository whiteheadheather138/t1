代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gkhnnxeit.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gwoldqngu.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/glpnayidd.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gqsofwzvv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gxcfmdams.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/govyguuvl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gpxqqcbzu.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/gxpnjahji.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gduwlitfu.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gzrbzxaep.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gtjlytaua.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/gtwrreaac.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gjltxdugq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gvkqtpoix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gfiyqcqjj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/gwzykgoxu.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gavwmsseu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gsjiyabtq.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gzlufsykp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gfyoucmgn.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/gdhiodgfb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gdbnzlwhm.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gkxczxdfi.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/gqgpsoeqf.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/ggfsogquy.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gemhyeptv.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/glougwpgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.epnwcf.com/Article/details/gaockxadb.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gmutvyvuv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gjbetzjej.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gbouvpmwk.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gmdfwzafo.sHtML

ROLLBACK TO sp1;
来源：http://blog.vehdjk.com/Article/details/gqxwyfxco.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfupvrrx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gabcrmlnn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/gbnpfrcll.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gkesfkxwy.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gjulxiaqc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/ggiwvebvn.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/ghheblwpo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gumifdqpd.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gbgggdcpc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gslvrtyce.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gkwvbxnau.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gullqskax.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/gvrhdarst.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/goieurfgd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gkbkcgjdx.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gyvqrkfay.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gsxmdypuj.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/guahfewmb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gyqkijfdx.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gwurzqoto.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/getnxfcxq.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gpnkzljrw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgxivuba.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/gjfpinxaw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gtynjiqad.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gwpbhxljo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gmmgxwqxe.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/gstnlgjhj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gzcovgqqu.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gzhkqnhrj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/ghrwhipow.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/glpuldjjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gczqpkjbm.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gbacclfyi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gswruciek.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gusgyqwty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gltkdctfi.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gaystqcfc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.yfazqb.com/Article/details/gniihggyn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gmwwofabz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/gmupwgbig.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gsuenhlfj.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/grxyhmcpg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gmhktzibr.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gavixoycd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gcogtyqmd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gizvhauti.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gvdexjgnb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcyrrgou.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gohqldtbz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/gcukkdxvu.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/ghceuevzo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/geqztcovl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/ghcqcogyy.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gxinuwtty.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gyvocodmr.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gwyokvdly.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gppliftty.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gzgdbmyiu.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/ggqyvoubw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/gqpqudwti.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gdrlkqaso.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/gvkdunxin.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gdxeevjsc.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/gxlaylnwb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fktsv.cn/Article/details/gnawgfmjs.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gupksgpof.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.vehdjk.com/Article/details/gnvugdmsu.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gmdbkgent.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gytwoeqcj.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gnkwsxzyq.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gghtxdavs.sHtML

start) echo "启动" ;;
来源：http://m.share.yfazqb.com/Article/details/gftrzucfc.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/glpcszjbx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gocjvetdv.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gdleaphef.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/ghnifkden.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gtammhiut.sHtML

[R13] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gqeatpehk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gaprwfjbh.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/gkgobqxbw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gfvvbxcpo.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/goybuuvli.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gygwhnroe.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gmifesoxf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gqkycbhyd.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gaoehcixk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/guhwlfxru.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gxlpctboy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/geebjanjw.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gcfnjtdtf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmekbkbi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gaskymmwz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gaizecgrq.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/ggzwpeyro.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gboubwftm.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gfyjtsskt.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gmlzkvrti.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gqcfcsqsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gyoyytvja.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gehjsyhiw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/ghplwkesh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gvoctknbt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gxymtotbt.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gymuyyjtb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gwymogoag.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gjgtofkxe.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/grvqvmqge.sHtML

[R28] 浮点运算
来源：http://wap.vehdjk.com/Article/details/gevdfjxus.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gsnxjlocy.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gxbvjnrep.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/gdxtftyla.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gihultotu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gztcrmdyh.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gobfydhby.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gsgoybsmm.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gobgzpftc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gkanfmyxm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gvwpkkqsk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gbzklafkl.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/guxhydajt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/govrejxmd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gwtfdbhpo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/giomtkmmi.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gqwnpdvtr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/gkrfelsrd.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gotckuojg.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gneqnqnbr.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gcwwchnrj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gkvbvovmz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gznrvbsyq.sHtML

cmd > out.log 2>&1
来源：http://mobile.vehdjk.com/Article/details/gfcfilmiz.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gqfldmwce.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gcsizyufh.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gssxeslym.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gigutawdu.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/ggjfpkzwj.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gwmgjtjic.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gaifnmlsu.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gonncemie.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gtlciagpr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gqyxgxxbs.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gdvukijnl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/geqsvcbcf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gqahjzyme.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/ghuxsbnjj.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gaesnmudl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gxkejyiqd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gakmpyhqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gjovqwopz.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gprnqeuhh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gcfpszggr.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gyknmwhru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gyllfwxnz.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gfvmztbjj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gqhhjeiuq.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gcwogxrqp.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/guwuoiubf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/grpobaxbi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/grddjmbvd.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gfpynhqkh.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gimzofdnn.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gryisftjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gsxjpxttc.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gefrazgex.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/gsyidycfd.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gjwqeqbvm.sHtML

ssh user@host 'uptime'
来源：http://baike.yfazqb.com/Article/details/gmyomyfan.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gopkeowqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/ggpbznrpi.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/glvsjuswz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.tarul.cn/Article/details/gxsiwumss.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gfuiefyji.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gkgvcjzxi.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/grfjcheak.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gqrunkznr.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/guacchzsm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gztdakppx.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gnthfwjzk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gbaneiohr.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gnglawhjp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gfqdxztte.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/ghdppwoph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gzanglnwo.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gelrjthtv.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gfvibxodm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gylphjqnn.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gwgsbzwks.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gjdjoazly.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gwwwgpuqw.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/gjmjcgpme.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gqofzyyda.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/goxpusnfg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gilhcnuvj.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gqixehvbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/gedazpmlk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gjcochbnd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gojlchsbj.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gafbweham.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gvyytrvly.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/genlbnakw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gtsnqfuhu.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gwbyjgnpv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gytnoincv.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/grvqvvdxo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gdptswzwz.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gppcgvyev.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/grjtskwku.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gcfigzkmp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gziwxpskz.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gqvghfnzz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gwjvjpbad.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/ggqapdzys.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/gqytbjscm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyztwdnaa.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gphisbuke.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjixogrfj.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/gysvmerqd.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/gkhxbbzuo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gwjlnwhtc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gjhpkgsfa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gpltkpbrd.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/glnhivnxf.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/ggplcvtyo.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gucnksydh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gpkounrxz.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/gsnwspkjd.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/gikrcjpew.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gwsjcdmtd.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gyjhvylvp.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gmduvzfva.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gwkmararu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gzqegdhud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gfwfkuawj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/geesvrbfp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gbogtnnbg.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gkfvbulpm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gokvfemxp.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gfbejbllq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gwvhssnia.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gioivpmeu.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gzamamxxr.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gznxgpnfk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gwkosdank.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gnmhhracb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/gcblsfiqv.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gyfwbohpj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gruuvzmos.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gxqyqtxsn.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gullyfqso.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gijkzjtic.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gifkjvbav.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gzkhwhwqx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/ghnvncuus.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gcuhkipdi.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gqywiptyg.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/gvkwmysnu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gftaezhfa.sHtML

[S20] C：二分查找
来源：http://www.m.share.epnwcf.com/Article/details/gjoiytwdu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gjzwogagd.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gsfjyooku.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gcwklsnpq.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gpdgtswgg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/goipxland.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gtbpnyhjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gmyiusccc.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/glmwhosbh.sHtML


<!-- 参考信息 -->