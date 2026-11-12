代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yfy.316326.xyz

) t WHERE rn = 1;
来源：http://vjq.jyoumei.cn

[Q35] 内连接
来源：http://aam.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gue.shanyushiyangtech.top

[Q36] 左连接
来源：http://iqo.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zhw.epnwcf.com

[Q37] 右连接
来源：http://lxp.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uma.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hhj.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kxy.tanke756.top

[Q39] 自连接（查上下级）
来源：http://gow.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hdc.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dvm.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://wxq.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hwk.havefunace.top

[Q41] 多表连接
来源：http://qts.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://buc.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://tig.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://xgz.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://zlx.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://sbq.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qbz.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://pab.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rcl.snrcjt.cn

[Q44] IN 子查询
来源：http://trq.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ykr.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://tkc.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ycz.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://wdg.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xgm.aibaodan.cn

[Q47] 与平均值比较
来源：http://nxp.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zsa.yj20258.top

[Q48] CTE 公用表表达式
来源：http://efc.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://etg.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://beq.yonumen.top

[Q49] 更新单行
来源：http://lmi.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://flj.sweek.top

[Q50] 批量更新
来源：http://cza.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tsl.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://byk.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pvp.shuidangran.top

[Q52] 删除指定行
来源：http://lcs.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://mjg.fktsv.cn

[Q53] 按条件删除
来源：http://iol.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yyy.zhixingplan.top

[Q54] 清空表
来源：http://fiu.sysykeji.top

TRUNCATE TABLE logs;
来源：http://ktz.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://fdi.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rhf.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://uyr.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ggc.xuanzx.com

[Q57] 行号
来源：http://bhv.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hyj.hysaishi.cn

[Q58] 累计求和
来源：http://moq.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hqt.gaohongyu789.top

[Q59] 分组内累计
来源：http://iev.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fyw.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://tam.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rmx.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://snr.chenlongwang.top

[Q61] 移动平均
来源：http://czg.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://muu.yanxiufei.cn

[Q62] 分组占比
来源：http://lgz.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mcr.havefunace.top

[Q63] 开启事务
来源：http://xyb.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qfl.gaohongyu789.top

[Q64] 提交事务
来源：http://sqm.aizwys.cn

COMMIT;
来源：http://krb.yuxming.cn

[Q65] 回滚事务
来源：http://gib.yj20258888.top

ROLLBACK;
来源：http://lsh.tanke756.top

[Q66] 行锁查询
来源：http://wvh.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fkc.tian-w.cn

[Q67] 设置隔离级别
来源：http://bbu.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eqx.ppjwa.cn

[Q68] 保存点
来源：http://lxf.zhijiandao.cn

SAVEPOINT sp1;
来源：http://rzr.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://rbq.guowangkeji.top

[Q69] 查看执行计划
来源：http://oyy.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://znx.havefunace.top

[Q70] 更新统计信息
来源：http://lwv.ybcxt.top

ANALYZE TABLE users;
来源：http://uwy.ivvv.top

[Q71] 查看建表语句
来源：http://hut.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ncq.shuidangran.top

[Q72] 查看索引
来源：http://sji.hesvh.cn

SHOW INDEX FROM users;
来源：http://xcn.ivvv.top

[Q73] 查看表状态
来源：http://szq.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://khz.tianlin.xyz

[Q74] 强制使用索引
来源：http://ilu.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rof.yanxiufei.cn

[Q75] 日期格式化
来源：http://llz.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gfw.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vhd.cashguo.top

[Q76] 按天统计
来源：http://oio.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://und.kuanghao11.cn

[Q77] 时间加减
来源：http://lng.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oxr.redwolf501.top

[Q78] 当前时间
来源：http://jey.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bxw.iojbl.cn

[Q79] 字符串拼接
来源：http://yjq.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nuy.yonumen.top

[Q80] 字符串截取
来源：http://nct.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xkl.shuidangran.top

[Q81] 字符串替换
来源：http://mul.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ane.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://agm.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lvd.guannengcc.top

[Q83] 大小写转换
来源：http://sfi.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sxz.ybcxt.top

[Q84] 去除首尾空格
来源：http://qoo.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://etp.yanxiufei.cn

[Q85] 数值取整
来源：http://maj.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oqz.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://gxv.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uzk.jianghu66.top

[Q87] JSON 字段做条件
来源：http://txb.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fjx.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://dqn.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://grs.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cjf.haohaochexian.top

[Q89] 判断表是否存在
来源：http://csq.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oaq.smart0.xyz

[Q90] 生成序号列
来源：http://oat.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nkd.kuanghao11.cn

================================================================================
来源：http://gni.andypj.xyz

R. Bash 专题
来源：http://cjr.vehdjk.com

================================================================================
来源：http://gkc.316326.xyz

[R01] shebang 与严格模式
来源：http://ers.birdmap.top

#!/usr/bin/env bash
来源：http://pem.uphjek.com

set -euo pipefail
来源：http://dtp.shuidangran.top

[R02] 变量赋值与使用
来源：http://vth.yfazqb.com

name="Tom"; echo "$name"
来源：http://ado.yj20258888.top

[R03] 只读变量
来源：http://cyh.jinghuilouyu.cn

readonly PI=3.14
来源：http://rtz.shangyingyoupin.top

[R04] 位置参数
来源：http://bmt.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hmq.jianghu66.top

[R05] 参数默认值
来源：http://iac.vehdjk.com

name="${1:-default}"
来源：http://yfd.aibaodan.cn

[R06] 判断命令是否存在
来源：http://efz.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qit.jqgufenzy.top

[R07] if 判断文件
来源：http://zae.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://krq.sjlbkw.cn

[R08] 数值比较
来源：http://yid.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://bvw.shanyushiyangtech.top

[R09] 字符串比较
来源：http://hdk.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://taq.xuetiantiany.cn

[R10] 正则匹配
来源：http://hva.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ktz.fehbvm.com

[R11] case 多分支
来源：http://hlj.nanxuanxn.top

case "$1" in
来源：http://hny.zycfv.cn

start) echo "启动" ;;
来源：http://mon.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://noo.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://rtj.shangyingyoupin.top

esac
来源：http://ckm.bbcook.cn

[R12] for 遍历文件
来源：http://emk.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://ydg.bjfxy.top

[R13] for 计数循环
来源：http://bda.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://oir.haohaochexian.top

[R14] C 风格 for
来源：http://fcq.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zpu.nanxuanxn.top

[R15] while 逐行读文件
来源：http://ydq.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mtf.shzxlz.cn

[R16] until 等待条件
来源：http://syy.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tan.chenzaomai.com

[R17] 数组定义与取值
来源：http://lzb.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://ndf.yueranfly.top

[R18] 遍历数组
来源：http://bzr.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oup.cheryme.top

[R19] 数组长度
来源：http://mvu.xuanzx.com

echo "${#arr[@]}"
来源：http://wve.ydzc1.top

[R20] 关联数组（字典）
来源：http://djl.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://meq.ppjwa.cn

[R21] 字符串长度
来源：http://jof.yj20258.top

echo "${#s}"
来源：http://lja.yj20258888.top

[R22] 截取子串
来源：http://fdk.fzhhl.top

echo "${s:0:5}"
来源：http://kaw.birdmap.top

[R23] 字符串替换
来源：http://jib.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xei.jinghuilouyu.cn

[R24] 大小写转换
来源：http://owh.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://fug.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://soc.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ple.fengsongda.top

[R26] 命令替换
来源：http://qmx.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://awv.jqgfzy.top

[R27] 算术展开
来源：http://pvo.epnwcf.com

echo $((1 + 2 * 3))
来源：http://wxa.jinghuilouyu.cn

[R28] 浮点运算
来源：http://tsd.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://sgj.wangdashe.top

[R29] 定义函数
来源：http://erz.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dic.hywenlv.cn

[R30] 函数返回状态码
来源：http://aac.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://xtc.fanxiaobao.xyz

[R31] 局部变量
来源：http://xgl.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://orq.fengsongda.top

[R32] 参数个数校验
来源：http://fbr.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cgb.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://vim.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bkj.snrcjt.cn

[R34] 退出时清理
来源：http://odk.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://yah.gotoacloud.top

[R35] 后台执行并等待
来源：http://dii.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jph.jqgfzy.top

[R36] 并发执行多个任务
来源：http://ixs.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nke.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://oct.cqqwz.cn

files=$(ls -1)
来源：http://iji.jiagoushi.top

[R38] 管道串联
来源：http://aot.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://gnm.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://vwi.gzhubu.top

cmd > out.log 2>&1
来源：http://xpl.shanyushiyangtech.top

[R40] 追加写日志
来源：http://wbv.zdqjudy.top

echo "log" >> out.log
来源：http://lci.dashuyun.cn

[R41] 丢弃输出
来源：http://jir.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://dww.zycfv.cn

[R42] 输入重定向
来源：http://gmg.ctjpmb.com

wc -l < a.txt
来源：http://ydw.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://wpj.redwolf501.top

find . -name "*.log" -type f
来源：http://iay.zdqjudy.top

[R44] 按修改时间查找
来源：http://xts.jqgufenzy.top

find . -mtime -7 -type f
来源：http://thu.xylfe.cn

[R45] 批量删除
来源：http://qny.wangdashe.top

find . -name "*.tmp" -delete
来源：http://jgf.nanxinkj.top

[R46] 递归替换文件内容
来源：http://qtj.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jih.yj202588.top

[R47] sed 单行替换
来源：http://bxe.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://yag.yuanzhike.top

[R48] awk 取指定列
来源：http://fak.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://trl.tian-w.cn

[R49] awk 带条件
来源：http://fag.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tib.0kj1m.cn

[R50] awk 求和
来源：http://mvl.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://yvh.yvedp.cn

[R51] 排序去重取前几
来源：http://tiz.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ezn.jiagoushi.top

[R52] 统计行数
来源：http://dre.cdnleiting.top

wc -l a.txt
来源：http://roc.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://dll.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://slq.sufxvd.cn

[R54] 比较两个文件
来源：http://zby.fehbvm.com

diff a.txt b.txt
来源：http://cvw.c1oappe.top

[R55] 压缩与解压
来源：http://fjb.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ove.hysaishi.cn

[R56] 远程拷贝
来源：http://ael.fktsv.cn

scp file user@host:/path/
来源：http://oqw.tarul.cn

[R57] 远程执行命令
来源：http://her.aizwys.cn

ssh user@host 'uptime'
来源：http://ecs.sufxvd.cn

[R58] 下载文件
来源：http://biq.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfy.fengsongda.top

[R59] 发 POST JSON
来源：http://lhu.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://crg.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://wke.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vqe.cheryme.top

[R61] 磁盘占用
来源：http://eun.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://bxs.dashuyun.cn

[R62] 找最占空间的文件
来源：http://iac.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://sba.yangfankeji.com

[R63] 内存与进程
来源：http://xgd.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://qqe.zhongyouzk.top

[R64] 结束进程
来源：http://iru.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://vxp.jianghu66.top

[R65] 查看端口占用
来源：http://atz.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yun.hongshengwenyu.top

[R66] 定时任务
来源：http://qmm.hcnkem.com

crontab -e;  crontab -l
来源：http://fee.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://uta.pycfn.com

openssl rand -hex 16
来源：http://clh.316326.xyz

[R68] 计算文件校验值
来源：http://olb.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://kox.9152youxi.cn

[R69] 生成随机密码
来源：http://gkw.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://lrp.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://nhu.xinyue.icu

date +%s;  date -d @1700000000
来源：http://wem.zhengqikj.top

[R71] 日期格式化
来源：http://kbj.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tyj.tarul.cn

[R72] 等待端口就绪
来源：http://ace.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zcq.316326.xyz

[R73] 分割大日志
来源：http://yio.zhixingplan.top

split -l 1000 big.log part_
来源：http://pdl.mhx1999.top

[R74] 批量重命名
来源：http://kmq.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lid.hnqzz.top

[R75] 导出环境变量
来源：http://gzy.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://nxw.guannengcc.top

[R76] 使用临时文件
来源：http://pjf.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xqo.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://gsu.haohaochexian.top

read -rp "请输入: " ans
来源：http://vyz.jqgfzy.top

[R78] 交互式菜单
来源：http://kym.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rrf.epnwcf.com

[R79] 解析命令行选项
来源：http://poh.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tak.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://mnj.tian-w.cn

time ./run.sh
来源：http://iys.zhixingplan.top

================================================================================
来源：http://hjw.hesvh.cn

S. C / C++ 专题
来源：http://nht.cdnleiting.top

================================================================================
来源：http://drd.bbcook.cn

[S01] C：Hello World
来源：http://hzj.fanxiaobao.xyz

#include <stdio.h>
来源：http://vdd.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ggw.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://ned.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://eeo.cashguo.top

[S03] C：读入整数
来源：http://bms.nwbrower.top


<!-- 参考信息 -->