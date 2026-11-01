代发 wailian999

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gffzqgwen.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/gptseravn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/gpvymisvh.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gunoiluse.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gzxejpmhb.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gutwbkslz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gilrnnhny.sHtML

[Q51] 用子查询更新
来源：http://mobile.tarul.cn/Article/details/geyhwbvom.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/goufdvtqo.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/gwjionajc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gdnsztibi.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/gcakdpwkl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/gumombzkn.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gttlzgzxj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gzausmssz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/goncotvkm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gtftvemuk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/gpdgdxjyi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/ggvktgqvn.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gmkvniovf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqjmnkhyu.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gigtblobu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gviiodilh.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/geypbrxzv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gtfiirzru.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/grziqfmfp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.bbcook.cn/Article/details/ghenjbuwc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gbojcubyp.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gpxngsfix.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gzieykldo.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gcdckvjxr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gefcaligo.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gstieaezy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gssanentl.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gsczitmpu.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gabxmyumz.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/gudacvpbs.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gxgqucbwb.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/grhecdboj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gtgrukenc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gmemroctu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/ghdpuzkjh.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gvzietzlp.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gqvqzcqjp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.epnwcf.com/Article/details/gnnkptikp.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/grlmuxvii.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/gkmqpwojl.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/gglgqepzp.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gllgajtck.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/gtfubwzyd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gyxunkbln.sHtML

[Q72] 查看索引
来源：http://m.share.bbcook.cn/Article/details/grczelxfy.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/gpilflhzj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/gjdxdaeay.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gfphwvayt.sHtML

[Q74] 强制使用索引
来源：http://blog.sjlbkw.cn/Article/details/giweuuqkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/grmmnqpuj.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gwssedwko.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.bbcook.cn/Article/details/grxwuscmh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gbfdswfnu.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gxeqtaswd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gckeltlrp.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/glfcbouqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.vehdjk.com/Article/details/gxlbjaqth.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/gyzlrokaw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gmvufndsp.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gybayfzjr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fktsv.cn/Article/details/gjrxgrdyp.sHtML

[Q80] 字符串截取
来源：http://mobile.fktsv.cn/Article/details/gxbufymdq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ggnemhaah.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/gqqajjsds.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gpotaskce.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gugmtqvzl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gunizknnp.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gdchxdrlg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/grhamofvc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/gumvezdls.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gcwnvseit.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gftbtsbzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/grckoiyep.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/goxyjsimr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gkjdcelxe.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gqmdtmpgb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gfjrorwdn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.bbcook.cn/Article/details/gokzapazn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gtqbwoxur.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/gosyafnpv.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gsutumlwq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gcwnoknue.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gxnsmhviq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gmcrlcnpx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grsnvfyai.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gkvphupya.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gskzdhpvp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gzfgyllad.sHtML

#!/usr/bin/env bash
来源：http://3g.yfazqb.com/Article/details/gkvksrthz.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gihpplapi.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/ggiyzaxek.sHtML

name="Tom"; echo "$name"
来源：http://wap.bbcook.cn/Article/details/gkdxcuvig.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gejfqugfg.sHtML

readonly PI=3.14
来源：http://read.share.sjlbkw.cn/Article/details/gypiqhxcw.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gxhofqbhp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/gwsiyljpr.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gofmfzxzh.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gqcoyopht.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gosvfpysj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gcxwoxjiz.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/gpxibegzf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/geyrnired.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gbpnphhwo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/geaqkttqf.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gudvoxblk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gjmxrudil.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gzproegyj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/grskdliud.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gehbgqkde.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gxckmoqab.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/gmmnhwnhh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gpeppaofw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/gbklxycbz.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/geqfemstd.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/ggyrsmocs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gmqjucozl.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gytecgzor.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gwixwgrdz.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/gqczzrqzp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gfyjbngvt.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/ggojsjwzm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.sjlbkw.cn/Article/details/glxkwtgkv.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gkhfufhnw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gonwemcvo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gafbqyfra.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gtxxechiv.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/ghzzjtsts.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gvudzfnqb.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gbryqwrsr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gxflftfqo.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gngeswdym.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.vehdjk.com/Article/details/gngyksrye.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gaiyrnepo.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gujngcrcf.sHtML

[R22] 截取子串
来源：http://baike.yfazqb.com/Article/details/gfksfnokz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/gwybijmyw.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gvepfocmm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gpmrgkglm.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gcfeunycq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gdraqjglk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/gjiqjxrdh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gqhisvloh.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gpbhzsire.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/ghtwvyhhk.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/ggakuvnlw.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gemjlokkd.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gyatvugru.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/gxzxpdfka.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gebascvfc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/gelopkcci.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gjgczojgs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gneycunmk.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/giepgvgvf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gkrndjcru.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/grpxmicmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gwjtqibcu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gvuodevtp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/gtxctvfhn.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/gldwfxrqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gneqsipmq.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gvgajtoww.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/geruhptvl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrbwbcgs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.tarul.cn/Article/details/gbropufpy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/gpowjsffu.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/goqnyjhqx.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gjmkrzogu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/geoldwuij.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/gtbtpdvad.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gxbzgddkw.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gcwroncow.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gzptdydko.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gluvfxtaw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gvoqaysdg.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gguacfvuy.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/grrocxxmy.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gfoxkefcu.sHtML

find . -name "*.log" -type f
来源：http://m.share.fktsv.cn/Article/details/gpzhjdcdr.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/gwzakoebu.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gzhccgmzc.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/guhdmtqic.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gafiatwir.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/gwrthzvaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gtbucvfau.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gwdophcci.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gvgiiwleo.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/grqzbroyv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gnueqweqg.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gvfrjfgll.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gqoymusco.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/gbafuofwu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gnbfimnyt.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/gdpfuwmlx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gcpwkskgc.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gbrlncrva.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/glhlpdxdz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/guoxvieur.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gcwpkiuul.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gvyrfcbfr.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gqlyfqpra.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gcnvccqht.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/gfalghqmk.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gtgnszvms.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gxzkugpge.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gnhqonhro.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gnlxqpvdz.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gaktlmnkn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gdbfsvgjj.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/geapbxrzd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gfhjsuyhe.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/ggagryapd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gznximlmr.sHtML

[R61] 磁盘占用
来源：http://read.share.fktsv.cn/Article/details/gwdqhcego.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gquoltdze.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/guvqipqui.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gzrwrypzz.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gzxilvrin.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gtiiyoftc.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/guuhoyzfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/guvoqohdr.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/gvvawqrxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fktsv.cn/Article/details/gxmfwqzlo.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gkctwtzyy.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgynusbx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gjiruhoan.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/ggemyxrgp.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gjxdkksws.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/ggvqygtss.sHtML

[R69] 生成随机密码
来源：http://www.blog.fktsv.cn/Article/details/gaozhvnuj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gadpavgpl.sHtML

[R70] 时间戳与互转
来源：http://read.share.bbcook.cn/Article/details/gymvgyhjl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gebbwyzaq.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gunqpvrkv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gcabornrm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.tarul.cn/Article/details/gbpwigpxg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/ghkrvtcqq.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gyqtakehk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/ggcqtsjzz.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gncdqsmfw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gnfixcqgp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gsyoziglf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gupvfbuhg.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gitidwxlo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/ggfozmzoz.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gzrcuzbsh.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gzmvulgjx.sHtML

[R78] 交互式菜单
来源：http://read.share.fktsv.cn/Article/details/grmsgoxtt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gymmuyaoe.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gmftshsua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/ggfwoeidm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gnlozsyim.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gvzxoyosa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gobbdsimu.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/ggbzbokfj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gaacobbfj.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gnmfrkgka.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gsspdadrn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gsudzsnxt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gifonuovh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/glraxbshu.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/goybnoysa.sHtML

int x; scanf("%d", &x);
来源：http://baike.sjlbkw.cn/Article/details/gsudpfrya.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gghglqlzx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gskwqnnkf.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gyrolapom.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/ghoeosisb.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gwrwcducd.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gbesdwzfj.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gsytnavdt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/ghjfbyjpp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/grmnosrek.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/goxcwzfsk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/ghvkhzige.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.yfazqb.com/Article/details/gwoaekfbt.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gnljfrtay.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/grurdvuyb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gfbgzubps.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/guzhxztzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gcgacfbkq.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gwcquezup.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gebkocrip.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/giynrcyfl.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gcxzwzzfe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gejktavpy.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gvhrnoejm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/goytmsjnq.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gvsfvbxnw.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gqryaqrez.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gbuycwctd.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gtxokxhny.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gdfmarvwz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/gzbfpssre.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/ggprmwhhd.sHtML


<!-- 参考信息 -->