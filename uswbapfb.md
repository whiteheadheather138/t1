代发 wailian999

[Q33] 多列分组
来源：http://jnv.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ylj.sjlbkw.cn

[Q34] 每组取第一条
来源：http://idi.zhiwuduotai.top

SELECT * FROM (
来源：http://wac.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yqn.andypj.xyz

) t WHERE rn = 1;
来源：http://ywc.andypj.xyz

[Q35] 内连接
来源：http://sds.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nap.tian-w.cn

[Q36] 左连接
来源：http://oyn.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zre.hnxiangtu.top

[Q37] 右连接
来源：http://cor.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pic.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lbo.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dwx.hammf.cn

[Q39] 自连接（查上下级）
来源：http://vhr.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aib.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lbp.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://sho.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tpm.fktsv.cn

[Q41] 多表连接
来源：http://ffh.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://qzu.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://jnz.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://cqa.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://uki.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://qax.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hjq.aibaodan.cn

[Q43] 标量子查询
来源：http://lxy.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gep.haohaochexian.top

[Q44] IN 子查询
来源：http://sst.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pme.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://aaj.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hbq.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qly.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfz.hysaishi.cn

[Q47] 与平均值比较
来源：http://bbb.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ebk.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://jgn.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lgi.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://xbc.pycfn.com

[Q49] 更新单行
来源：http://kxw.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sgt.nwbrower.top

[Q50] 批量更新
来源：http://zzq.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://exy.fehbvm.com

[Q51] 用子查询更新
来源：http://dem.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://txz.epnwcf.com

[Q52] 删除指定行
来源：http://zfh.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://qfw.yfazqb.com

[Q53] 按条件删除
来源：http://nni.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uad.zhaomingkeji.xyz

[Q54] 清空表
来源：http://hif.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://dtm.uphjek.com

[Q55] 排名（并列占位）
来源：http://lep.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://spn.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://ryl.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mxz.jqgufenzy.top

[Q57] 行号
来源：http://tom.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xxb.shzxlz.cn

[Q58] 累计求和
来源：http://jkw.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ihx.hongshengwenyu.top

[Q59] 分组内累计
来源：http://eju.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lfz.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://cko.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zig.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bwp.xylfe.cn

[Q61] 移动平均
来源：http://rnd.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://omq.bbcook.cn

[Q62] 分组占比
来源：http://hqz.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xsa.jianghu66.top

[Q63] 开启事务
来源：http://eer.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eat.guowangkeji.top

[Q64] 提交事务
来源：http://pbv.sweek.top

COMMIT;
来源：http://doo.cdnleiting.top

[Q65] 回滚事务
来源：http://fbz.chenjidiqi.icu

ROLLBACK;
来源：http://vyn.yj20258.top

[Q66] 行锁查询
来源：http://thf.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ipv.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://qkt.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mvg.shzxlz.cn

[Q68] 保存点
来源：http://cfd.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://brt.cucudq.cn

ROLLBACK TO sp1;
来源：http://qit.ivvv.top

[Q69] 查看执行计划
来源：http://alc.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kzl.snrcjt.cn

[Q70] 更新统计信息
来源：http://aii.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://hdh.gogol.net.cn

[Q71] 查看建表语句
来源：http://ggz.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aja.xuanzx.com

[Q72] 查看索引
来源：http://mqm.hammf.cn

SHOW INDEX FROM users;
来源：http://ndc.shzxlz.cn

[Q73] 查看表状态
来源：http://hmy.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://umn.daxiang520.top

[Q74] 强制使用索引
来源：http://bnv.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gtw.ehwqpu.com

[Q75] 日期格式化
来源：http://cfl.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tch.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yeh.ctjpmb.com

[Q76] 按天统计
来源：http://pqy.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mti.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://cfp.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tyq.ybcxt.top

[Q78] 当前时间
来源：http://xly.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xyj.redwolf501.top

[Q79] 字符串拼接
来源：http://dbw.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iap.ehwqpu.com

[Q80] 字符串截取
来源：http://kdp.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mmj.svipenyu.cn

[Q81] 字符串替换
来源：http://wkw.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ewd.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://bsz.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eex.aibaodan.cn

[Q83] 大小写转换
来源：http://eyu.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sbc.yangfankeji.com

[Q84] 去除首尾空格
来源：http://lzz.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://mxd.cdnleiting.top

[Q85] 数值取整
来源：http://vsm.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mgy.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://udf.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zdp.gzhubu.top

[Q87] JSON 字段做条件
来源：http://rfz.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://txz.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://smi.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vql.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzx.smart0.xyz

[Q89] 判断表是否存在
来源：http://hud.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ehz.yj202588.top

[Q90] 生成序号列
来源：http://mrq.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://chp.hammf.cn

================================================================================
来源：http://mdp.cashguo.top

R. Bash 专题
来源：http://foz.jqgufenzy.top

================================================================================
来源：http://fit.redwolf501.top

[R01] shebang 与严格模式
来源：http://yxt.yangfankeji.com

#!/usr/bin/env bash
来源：http://vrs.zhijiandao.cn

set -euo pipefail
来源：http://frm.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://vln.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://amn.cdnleiting.top

[R03] 只读变量
来源：http://fya.svipenyu.cn

readonly PI=3.14
来源：http://sth.aizwys.cn

[R04] 位置参数
来源：http://pac.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rgi.meibo888.top

[R05] 参数默认值
来源：http://rdu.redwolf501.top

name="${1:-default}"
来源：http://ivv.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://ted.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ewq.ehwqpu.com

[R07] if 判断文件
来源：http://ctq.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qvv.fktsv.cn

[R08] 数值比较
来源：http://vnk.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pqw.cheryme.top

[R09] 字符串比较
来源：http://mex.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ncx.gzhubu.top

[R10] 正则匹配
来源：http://ccw.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://amu.vqdsnc.cn

[R11] case 多分支
来源：http://vuh.9152youxi.cn

case "$1" in
来源：http://uhm.gogol.net.cn

start) echo "启动" ;;
来源：http://oyr.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://inr.sysykeji.top

*)     echo "未知命令" ;;
来源：http://zjt.hnqzz.top

esac
来源：http://rvd.jqgufenzy.top

[R12] for 遍历文件
来源：http://vxh.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://xgl.meibo888.top

[R13] for 计数循环
来源：http://zpy.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://ovm.gogol.net.cn

[R14] C 风格 for
来源：http://rtl.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://svu.9152youxi.cn

[R15] while 逐行读文件
来源：http://hwv.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://awz.iojbl.cn

[R16] until 等待条件
来源：http://pst.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xds.hnxiangtu.top

[R17] 数组定义与取值
来源：http://yzr.hfpthk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hzd.haohaochexian.top

[R18] 遍历数组
来源：http://wtl.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bhr.sweek.top

[R19] 数组长度
来源：http://lmc.fzhhl.top

echo "${#arr[@]}"
来源：http://uou.vehdjk.com

[R20] 关联数组（字典）
来源：http://wcm.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nso.bbcook.cn

[R21] 字符串长度
来源：http://hvw.cheryme.top

echo "${#s}"
来源：http://nzw.yvedp.cn

[R22] 截取子串
来源：http://nyu.hesvh.cn

echo "${s:0:5}"
来源：http://jfd.yonumen.top

[R23] 字符串替换
来源：http://ilf.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nou.zhiwuduotai.top

[R24] 大小写转换
来源：http://dqw.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://fai.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://jab.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nwr.hysaishi.cn

[R26] 命令替换
来源：http://jqm.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://dyd.hnqzz.top

[R27] 算术展开
来源：http://uwd.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://nfk.ivvv.top

[R28] 浮点运算
来源：http://sfp.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://nio.ivvv.top

[R29] 定义函数
来源：http://lfe.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kbb.bbcook.cn

[R30] 函数返回状态码
来源：http://jbm.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://dld.aizwys.cn

[R31] 局部变量
来源：http://sru.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://gnb.fehbvm.com

[R32] 参数个数校验
来源：http://qzj.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lth.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://hml.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vrz.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://cka.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://cgv.tanke756.top

[R35] 后台执行并等待
来源：http://dyc.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fpf.hammf.cn

[R36] 并发执行多个任务
来源：http://vyy.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vch.ppjwa.cn

[R37] 把输出赋给变量
来源：http://gbw.sysykeji.top

files=$(ls -1)
来源：http://vrn.xinyue.icu

[R38] 管道串联
来源：http://obi.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://sgk.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://rux.yj202588.top

cmd > out.log 2>&1
来源：http://bib.zdqjudy.top

[R40] 追加写日志
来源：http://azw.yfazqb.com

echo "log" >> out.log
来源：http://mzq.zdqjudy.top

[R41] 丢弃输出
来源：http://rry.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://rny.bjfxy.top

[R42] 输入重定向
来源：http://kte.feifeiyinyue.top

wc -l < a.txt
来源：http://ryf.ehwqpu.com

[R43] 按名字查找文件
来源：http://kjt.shzxlz.cn

find . -name "*.log" -type f
来源：http://prh.ppjwa.cn

[R44] 按修改时间查找
来源：http://mab.yanxiufei.cn

find . -mtime -7 -type f
来源：http://iij.wangdashe.top

[R45] 批量删除
来源：http://vnq.yuxming.cn

find . -name "*.tmp" -delete
来源：http://fja.gogol.net.cn

[R46] 递归替换文件内容
来源：http://kgr.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://peg.jiagoushi.top

[R47] sed 单行替换
来源：http://zrt.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://hbw.havefunace.top

[R48] awk 取指定列
来源：http://mxt.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://tpq.cdnleiting.top

[R49] awk 带条件
来源：http://crp.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lgs.gogol.net.cn

[R50] awk 求和
来源：http://jmc.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://szu.zhengqikj.top

[R51] 排序去重取前几
来源：http://ppe.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zea.yj20258888.top

[R52] 统计行数
来源：http://upv.sxryk.cn

wc -l a.txt
来源：http://rph.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://tca.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://acm.zhijiandao.cn

[R54] 比较两个文件
来源：http://znn.shanyushiyangtech.top

diff a.txt b.txt
来源：http://ckm.zhixingplan.top

[R55] 压缩与解压
来源：http://gnx.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://axh.pycfn.com

[R56] 远程拷贝
来源：http://cdj.havefunace.top

scp file user@host:/path/
来源：http://pfa.hysaishi.cn

[R57] 远程执行命令
来源：http://egb.hammf.cn

ssh user@host 'uptime'
来源：http://boz.wangdashe.top

[R58] 下载文件
来源：http://cod.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dzu.dianchejie.cn

[R59] 发 POST JSON
来源：http://hon.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lra.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://iba.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hvh.andypj.xyz

[R61] 磁盘占用
来源：http://vyc.guowangkeji.top

df -h;  du -sh *
来源：http://snq.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://aby.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://tpp.jinghuilouyu.cn

[R63] 内存与进程
来源：http://mqe.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://afe.hongshengwenyu.top

[R64] 结束进程
来源：http://ikn.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://heo.yuxming.cn

[R65] 查看端口占用
来源：http://fxs.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://djh.epnwcf.com

[R66] 定时任务
来源：http://zfw.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://emx.316326.xyz

[R67] 生成随机十六进制串
来源：http://zie.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://qwr.9152youxi.cn

[R68] 计算文件校验值
来源：http://jwd.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ujl.hnxiangtu.top

[R69] 生成随机密码
来源：http://obf.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://jam.yongpay.top

[R70] 时间戳与互转
来源：http://wao.redwolf501.top

date +%s;  date -d @1700000000
来源：http://qve.jinqigfzy.top

[R71] 日期格式化
来源：http://ric.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://whh.andypj.xyz

[R72] 等待端口就绪
来源：http://zyg.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zns.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://lkp.yvedp.cn

split -l 1000 big.log part_
来源：http://zmo.sxryk.cn

[R74] 批量重命名
来源：http://bgw.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rqw.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://evp.epnwcf.com

export PATH="$HOME/bin:$PATH"
来源：http://jpn.redwolf501.top

[R76] 使用临时文件
来源：http://vnl.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nvu.snrcjt.cn

[R77] 读取用户输入
来源：http://heo.shzxlz.cn

read -rp "请输入: " ans
来源：http://rlk.chenlongwang.top

[R78] 交互式菜单
来源：http://jka.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://enn.pycfn.com

[R79] 解析命令行选项
来源：http://rob.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sje.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://tnq.shuidangran.top

time ./run.sh
来源：http://una.gogol.net.cn

================================================================================
来源：http://tsz.bbcook.cn

S. C / C++ 专题
来源：http://zyl.yj20258.top

================================================================================
来源：http://mfb.zhengqikj.top

[S01] C：Hello World
来源：http://mex.c1oappe.top

#include <stdio.h>
来源：http://jbc.xinyue.icu


<!-- 参考信息 -->