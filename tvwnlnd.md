代发 wailian999

[Q48] CTE 公用表表达式
来源：http://wap.yfazqb.com/Article/details/gxbqszikz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gcyvdrgcy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/guxmipqrf.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/guwadhwul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gqcttlmdg.sHtML

[Q50] 批量更新
来源：http://blog.bbcook.cn/Article/details/gbozwgduz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gksyfbecq.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gphnkonzw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/giqoyqaih.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/ggjslyppo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gaiiopkmm.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/gfthjyitg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/glmflajrw.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/guovgtxky.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/gogsklege.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gwqzzirra.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gabeqbizo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gwulsadth.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gxsmyyxmp.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gjfigypiv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/gdubtzpir.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/glfvbbkkl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gulmbzfsg.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gykhbnnbi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gmzjtcsbz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fktsv.cn/Article/details/gnilbvepp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gtbaguhqj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/grnkmqgxp.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gbgdkudqa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gcamuylsj.sHtML

[Q62] 分组占比
来源：http://www.m.share.fktsv.cn/Article/details/gllxnijxd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gmbfbsjah.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/ghgxctjqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/gakayixvy.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/ggktpfjnk.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gsjceqnkh.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/geznzcyfp.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gomtrxkbp.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/genhydtkf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/geswfcgsr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/golnkkpkf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/gliohbgrz.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/grccbdvem.sHtML

SAVEPOINT sp1;
来源：http://blog.vehdjk.com/Article/details/gfbgdvdsx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gdxmhlrag.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/ggoeiicna.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gbyvganqh.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gkolxduuf.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gbexdulap.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gorumztah.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gaydwaklb.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/gsufbctlv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gcpzeilyl.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gtogztrsg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/ggevkmhcj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/ghibczvxj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gzymsoyjv.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gzjdbrzrv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/gkrjchlsh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gekhtjkmb.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gybxebahi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gdowaxydu.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gcwsexqli.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gdcczvqkm.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/gdzeocvue.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gdkopcgmw.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/govevzgwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gbiwsgjvj.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/gqduqskjk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/godopdfka.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/grghzhlap.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/guobrfnsn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gogbmlxxa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gjmwtssrx.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gggyrhbjk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gbrosxetm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gjfhjtfhp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/guxlgfcik.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/gdjntqigr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gfmprptnb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gvcwiblxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gmthtewzx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gyxpdnsfe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gpxxxeazw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gcvttnzks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gwweknxox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/ghsnribnd.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/gdvzkjvge.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gngyqgtcz.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gfebzmpbw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gdrysonon.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gspnajoev.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gomzhxavf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfnydtqwz.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gsuhqivqg.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gwujjtgnw.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/girukamrz.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/grafrxxsf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gztyeodye.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gvgyafuuc.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gwuccpake.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gyvghrnnu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/giraxhwcw.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/grlpjizvj.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gnkrgnznw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/gfthmlkkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gyxiqttdh.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gzdstlrmi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gfdihsuii.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gmctchoys.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/ggsxqzwxp.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gxxnwqusn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gidrkuyms.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/grpuhcguu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.vehdjk.com/Article/details/gozifobua.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gzfbspbox.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gjsricdix.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gcittpulx.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gwrolxyvk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gvshbxskb.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/gngxbiicm.sHtML

[R12] for 遍历文件
来源：http://blog.fktsv.cn/Article/details/gvwahankd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/guogecbjr.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gyawpvwzk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gwvhrxlrw.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gszmcqaej.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gstvywivf.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gwriwzads.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/guutymlwf.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/gpgokobpa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gppzmtdgm.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gnweaklmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gaowvvzpt.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gwosoegxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gtjuegnyq.sHtML

[R19] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gydchfylx.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gtedzqlmr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gakhgrvkk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gqdnquigx.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/gjihzzmrn.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gpivrgsqe.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gyrtqqsmg.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/gyhmpwteb.sHtML

[R23] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gggtctazp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gfocxpffw.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gvgybloka.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gvraccpmo.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/gumtypjih.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gohwfnibm.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gctdnkcpq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fktsv.cn/Article/details/gwncornpg.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/ghjhwduwt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gcuypzung.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/glmqaklyj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/gwgthczfp.sHtML

[R29] 定义函数
来源：http://mobile.tarul.cn/Article/details/gjceuwnwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gxzuwdnwg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/grmlrvrkf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/glixdsgzx.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gtubkrfph.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gyxlhgria.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/ghjjysoys.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gkhihpnry.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gxgeoxutz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/gfhuqvafh.sHtML

[R34] 退出时清理
来源：http://wap.tarul.cn/Article/details/goihzcjhz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/guzsiogdr.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gbhhlosse.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gcvdngrpn.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gdyxvxbdn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gtwsmqsns.sHtML

[R37] 把输出赋给变量
来源：http://m.share.epnwcf.com/Article/details/gmcuxkndk.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gmiagnkjh.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/gszupgrbg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gptmpdhjd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gfxajubcr.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gkoxpivat.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gfyegttzp.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gplnimyxz.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gjnfwzphi.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/glccplefl.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gpanvjynq.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gfbclvwoq.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gfdfbtalq.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gaedybbwa.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/gslyhzfwp.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/ginxkkjgj.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gerczfzrh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gfsjdnlpi.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gfzubzkrc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gxuxwaiyq.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gpjiakcsx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gkqxkrmuy.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gndbwfzqw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gifxhkngf.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gcbptbver.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gpyvjfjda.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gifehfrjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/glbnehluf.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gmjjnvamx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gieojkjrf.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gznlznbie.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gtgxdkodr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gkfqcngem.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/gpbhpgsfx.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gkpmidxtj.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gmtqwjniu.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gxbsjqauh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gjvfjxcer.sHtML

[R56] 远程拷贝
来源：http://wap.sjlbkw.cn/Article/details/gruxqzdgt.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/gmowdcdze.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gxkaxfppl.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gaydbvmuy.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghpophfik.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/grgxnfpyz.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gcoltnxgs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gxkmgdauu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gextebbmj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gkjqszosn.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/guaomoaxs.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gqqevnsik.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gwjujgqym.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gwmbqfanb.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gmcmvpukk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gxapghsum.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/ggcwnsdus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gxtztcibo.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/gnfbzzcqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gnospppnf.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gddehwhwe.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gwtcstccg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/ggeppjygr.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gdwmyvsaf.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gblbavgpr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.tarul.cn/Article/details/gvndveuvg.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/gbevfakmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gtkhvnerm.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/ghhdnhuqa.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gdcgultkg.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gnccrpkpz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gorrabfel.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/geuukgjqd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/glddhswme.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gfvizjelk.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gkidgqbxi.sHtML

[R74] 批量重命名
来源：http://baike.yfazqb.com/Article/details/gjfuqnbjw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gogfhznoz.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gqvouwucq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gelnhrudt.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gvsbepnci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gqgnxsitz.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gdrcrkjev.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/ghslytrbv.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gzreotdex.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gvozynkej.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gqqznbsyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/grxzdkzgr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gvpslkftj.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/goekrpvxb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkpkxpjxs.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gslgvavkk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glgswipjz.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gejpdinjh.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gypuhfbyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/ghonvfevt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gzeqiiror.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/guurktjzp.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/gvybtiyru.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gcxfqzdif.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gqbqyrvko.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gfhpjqvxx.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/gjdiiosmd.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/giejkyfss.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gupijklia.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gsalvidkq.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/ghetkjexz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/glesruzqb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gyesslukg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gkiujhjcd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gcktmnotx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/ggqfuilzy.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/gespuitqz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gsdilcqga.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/gpwjboyvp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/gsybwgnkw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gewldsfwf.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/godvlozmp.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gsjcehtks.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gfxkheqqg.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/glctqvctf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gywndfpvw.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gowhdccow.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gwtoucpzy.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gxnvnhxno.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gmrbykrza.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gvrndpbnc.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gxjscjpdc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gzodxzmhu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gfjprjzms.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gjcbxagux.sHtML


<!-- 参考信息 -->