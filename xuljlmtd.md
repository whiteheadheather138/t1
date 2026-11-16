代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xrh.yuanzhike.top

[Q26] 计数
来源：http://nzx.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://pfl.daria6918.cn

[Q27] 条件计数
来源：http://jkk.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mde.jinqigufen.top

[Q28] 求和与平均
来源：http://slm.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xlh.316326.xyz

[Q29] 最大最小值
来源：http://zxc.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fqd.0kj1m.cn

[Q30] 分组统计
来源：http://puo.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://izg.aibaodan.cn

[Q31] 分组后过滤
来源：http://fyr.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mzf.c1oappe.top

[Q32] 分组拼接字符串
来源：http://sic.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ijo.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ifw.yj20258888.top

[Q33] 多列分组
来源：http://gxv.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mne.jiagoushi.top

[Q34] 每组取第一条
来源：http://lyl.snrcjt.cn

SELECT * FROM (
来源：http://bhu.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://onx.vqdsnc.cn

) t WHERE rn = 1;
来源：http://ksr.cqqwz.cn

[Q35] 内连接
来源：http://cme.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uwq.gotoacloud.top

[Q36] 左连接
来源：http://alf.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vil.chenjidiqi.icu

[Q37] 右连接
来源：http://lxn.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pfr.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://tvd.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dhg.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://lft.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xag.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jpf.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://kmj.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jqz.zdbjq.cn

[Q41] 多表连接
来源：http://xgc.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ozv.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://zap.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://cgg.birdmap.top

[Q42] 连接条件附加过滤
来源：http://siz.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://dce.uphjek.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vsf.xylfe.cn

[Q43] 标量子查询
来源：http://zoa.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xbs.52xcode.cn

[Q44] IN 子查询
来源：http://boa.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wyh.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://crd.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ubv.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://xjn.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dsz.pycfn.com

[Q47] 与平均值比较
来源：http://zjj.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mqm.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://gys.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://stc.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://ims.nwbrower.top

[Q49] 更新单行
来源：http://rrt.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ibj.ehwqpu.com

[Q50] 批量更新
来源：http://yem.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rza.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://nyp.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zfk.sweek.top

[Q52] 删除指定行
来源：http://cqx.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://jws.ehwqpu.com

[Q53] 按条件删除
来源：http://qoh.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://boi.cdnleiting.top

[Q54] 清空表
来源：http://dfx.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://vcd.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://rll.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://omr.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://ntr.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wrb.wangdashe.top

[Q57] 行号
来源：http://gku.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uos.fanxiaobao.xyz

[Q58] 累计求和
来源：http://uon.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ioz.gogol.net.cn

[Q59] 分组内累计
来源：http://icu.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://far.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://buj.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://txu.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dgq.gotoacloud.top

[Q61] 移动平均
来源：http://fgl.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dch.chenzaomai.com

[Q62] 分组占比
来源：http://ier.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://moy.chenjidiqi.icu

[Q63] 开启事务
来源：http://iff.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hvy.tanke756.top

[Q64] 提交事务
来源：http://eox.shanyushiyangtech.top

COMMIT;
来源：http://kpr.xuanzx.com

[Q65] 回滚事务
来源：http://txk.jqgufenzy.top

ROLLBACK;
来源：http://uvn.yvedp.cn

[Q66] 行锁查询
来源：http://obq.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sgy.cucudq.cn

[Q67] 设置隔离级别
来源：http://bhg.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zsz.cucudq.cn

[Q68] 保存点
来源：http://exk.gaohongyu789.top

SAVEPOINT sp1;
来源：http://gps.epnwcf.com

ROLLBACK TO sp1;
来源：http://qjk.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://szt.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ywe.yanxiufei.cn

[Q70] 更新统计信息
来源：http://hah.nanxinkj.top

ANALYZE TABLE users;
来源：http://ujl.yanxiufei.cn

[Q71] 查看建表语句
来源：http://xoe.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uxr.cucudq.cn

[Q72] 查看索引
来源：http://ull.hfpthk.cn

SHOW INDEX FROM users;
来源：http://ivo.ydjk.org.cn

[Q73] 查看表状态
来源：http://idx.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wsh.guowangkeji.top

[Q74] 强制使用索引
来源：http://ozk.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xrb.tarul.cn

[Q75] 日期格式化
来源：http://ekr.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uep.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zkx.316326.xyz

[Q76] 按天统计
来源：http://okm.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://owp.birdmap.top

[Q77] 时间加减
来源：http://hni.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ajm.gzhubu.top

[Q78] 当前时间
来源：http://xks.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qxg.cucudq.cn

[Q79] 字符串拼接
来源：http://bwv.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rex.guannengcc.top

[Q80] 字符串截取
来源：http://nnv.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://koe.guannengcc.top

[Q81] 字符串替换
来源：http://kgj.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fkx.hammf.cn

[Q82] 字符长度与字节长度
来源：http://tmm.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hmu.zdqjudy.top

[Q83] 大小写转换
来源：http://wgm.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ogp.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://adx.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://whf.jqgufenzy.top

[Q85] 数值取整
来源：http://qsu.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jgx.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://dqw.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://loy.ydzc1.top

[Q87] JSON 字段做条件
来源：http://fdi.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lmm.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://jak.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uyj.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fun.c1oappe.top

[Q89] 判断表是否存在
来源：http://egi.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dvq.snrcjt.cn

[Q90] 生成序号列
来源：http://oug.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qoa.ybcxt.top

================================================================================
来源：http://vaf.ehwqpu.com

R. Bash 专题
来源：http://sqw.yueranfly.top

================================================================================
来源：http://zgv.nwbrower.top

[R01] shebang 与严格模式
来源：http://waw.9152youxi.cn

#!/usr/bin/env bash
来源：http://twu.yuanzhike.top

set -euo pipefail
来源：http://xhm.tian-w.cn

[R02] 变量赋值与使用
来源：http://jgi.chenzaomai.com

name="Tom"; echo "$name"
来源：http://wae.fanxiaobao.xyz

[R03] 只读变量
来源：http://vta.andypj.xyz

readonly PI=3.14
来源：http://ixe.shuidangran.top

[R04] 位置参数
来源：http://lka.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qau.316326.xyz

[R05] 参数默认值
来源：http://xsj.yuxming.cn

name="${1:-default}"
来源：http://djw.vehdjk.com

[R06] 判断命令是否存在
来源：http://vql.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://grg.chenlongwang.top

[R07] if 判断文件
来源：http://pvd.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pqy.pengpengdd.cyou

[R08] 数值比较
来源：http://uah.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fue.yongpay.top

[R09] 字符串比较
来源：http://hsr.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wmg.zhoulong.xyz

[R10] 正则匹配
来源：http://kif.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bww.yfazqb.com

[R11] case 多分支
来源：http://xqz.zhoulong.xyz

case "$1" in
来源：http://iiv.shangyingyoupin.top

start) echo "启动" ;;
来源：http://nwb.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://uvl.yonumen.top

*)     echo "未知命令" ;;
来源：http://izu.mhx1999.top

esac
来源：http://btt.chenjidiqi.icu

[R12] for 遍历文件
来源：http://txn.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://lpo.tianlin.xyz

[R13] for 计数循环
来源：http://qam.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://tlt.fengsongda.top

[R14] C 风格 for
来源：http://xhs.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tfb.jinqigufen.top

[R15] while 逐行读文件
来源：http://tdr.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gkh.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://wyx.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jlf.tanke756.top

[R17] 数组定义与取值
来源：http://npm.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://whq.feifeiyinyue.top

[R18] 遍历数组
来源：http://xjh.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://glz.316326.xyz

[R19] 数组长度
来源：http://wpz.yfazqb.com

echo "${#arr[@]}"
来源：http://hwp.daria6918.cn

[R20] 关联数组（字典）
来源：http://vvc.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://plv.haohaochexian.top

[R21] 字符串长度
来源：http://uuy.fzhhl.top

echo "${#s}"
来源：http://blb.sweek.top

[R22] 截取子串
来源：http://wty.sysykeji.top

echo "${s:0:5}"
来源：http://edu.yueranfly.top

[R23] 字符串替换
来源：http://dln.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pre.jlsjyb.cn

[R24] 大小写转换
来源：http://ike.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nkl.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://wiy.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sjb.ydjk.org.cn

[R26] 命令替换
来源：http://pmb.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://vmt.yongpay.top

[R27] 算术展开
来源：http://aut.dianchejie.cn

echo $((1 + 2 * 3))
来源：http://twx.zhongyouzk.top

[R28] 浮点运算
来源：http://vft.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://yij.daxiang520.top

[R29] 定义函数
来源：http://bva.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://imi.hnqzz.top

[R30] 函数返回状态码
来源：http://grd.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://spr.zycfv.cn

[R31] 局部变量
来源：http://ggd.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://slj.jlsjyb.cn

[R32] 参数个数校验
来源：http://yxb.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lbx.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://ysk.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wqm.uphjek.com

[R34] 退出时清理
来源：http://qgc.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yzf.cqqwz.cn

[R35] 后台执行并等待
来源：http://jsw.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xtn.sysykeji.top

[R36] 并发执行多个任务
来源：http://vnt.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jub.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://luy.tarul.cn

files=$(ls -1)
来源：http://myk.hfpthk.cn

[R38] 管道串联
来源：http://vkl.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://ami.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://qgr.tarul.cn

cmd > out.log 2>&1
来源：http://rft.aizwys.cn

[R40] 追加写日志
来源：http://cox.ydzc1.top

echo "log" >> out.log
来源：http://odg.hnqzz.top

[R41] 丢弃输出
来源：http://oyt.shuidangran.top

cmd >/dev/null 2>&1
来源：http://jvh.zhongyouzk.top

[R42] 输入重定向
来源：http://lzd.316326.xyz

wc -l < a.txt
来源：http://qiq.nwbrower.top

[R43] 按名字查找文件
来源：http://tdk.ydjk.org.cn

find . -name "*.log" -type f
来源：http://tfo.fktsv.cn

[R44] 按修改时间查找
来源：http://nzw.shuidangran.top

find . -mtime -7 -type f
来源：http://qrv.cashguo.top

[R45] 批量删除
来源：http://raz.yuxming.cn

find . -name "*.tmp" -delete
来源：http://xne.52xcode.cn

[R46] 递归替换文件内容
来源：http://yss.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rha.sufxvd.cn

[R47] sed 单行替换
来源：http://una.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hdm.cashguo.top

[R48] awk 取指定列
来源：http://dre.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://ztn.feifeiyinyue.top

[R49] awk 带条件
来源：http://kiy.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oqn.yueranfly.top

[R50] awk 求和
来源：http://whk.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://giu.cucudq.cn

[R51] 排序去重取前几
来源：http://wny.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dbc.gogol.net.cn

[R52] 统计行数
来源：http://fxt.yueranfly.top

wc -l a.txt
来源：http://zjn.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://ycj.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wty.sysykeji.top

[R54] 比较两个文件
来源：http://abt.jinqigufen.top

diff a.txt b.txt
来源：http://crp.sysykeji.top

[R55] 压缩与解压
来源：http://vky.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bee.ivvv.top

[R56] 远程拷贝
来源：http://vom.smart0.xyz

scp file user@host:/path/
来源：http://zzj.vqdsnc.cn

[R57] 远程执行命令
来源：http://lhf.birdmap.top

ssh user@host 'uptime'
来源：http://zbn.andypj.xyz

[R58] 下载文件
来源：http://lqs.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bfz.wangdashe.top

[R59] 发 POST JSON
来源：http://uik.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fmd.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://gfd.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gsf.yfazqb.com

[R61] 磁盘占用
来源：http://grs.sufxvd.cn

df -h;  du -sh *
来源：http://mly.yongpay.top

[R62] 找最占空间的文件
来源：http://uok.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://dkv.tanke756.top

[R63] 内存与进程
来源：http://gzn.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://xym.dashuyun.cn

[R64] 结束进程
来源：http://qbe.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://xmt.nanxinkj.top

[R65] 查看端口占用
来源：http://mcd.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://arg.aibaodan.cn

[R66] 定时任务
来源：http://ons.guannengcc.top

crontab -e;  crontab -l
来源：http://shg.sxryk.cn

[R67] 生成随机十六进制串
来源：http://ada.tian-w.cn

openssl rand -hex 16
来源：http://bjk.zhijiandao.cn

[R68] 计算文件校验值
来源：http://rbn.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iqy.ydjk.org.cn

[R69] 生成随机密码
来源：http://aod.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://htt.cashguo.top

[R70] 时间戳与互转
来源：http://ldf.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://hnp.fanxiaobao.xyz

[R71] 日期格式化
来源：http://ieg.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://sxl.jlsjyb.cn

[R72] 等待端口就绪
来源：http://zar.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://foo.wangdashe.top

[R73] 分割大日志
来源：http://bya.hfpthk.cn

split -l 1000 big.log part_
来源：http://qwz.yangfankeji.com

[R74] 批量重命名
来源：http://zny.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://htz.yonumen.top

[R75] 导出环境变量
来源：http://wsx.jinyuanbaomall.cn


<!-- 参考信息 -->