代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://xjv.hywenlv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gjb.yuanzhike.top

[Q13] 忽略重复插入
来源：http://tgw.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qzo.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://tpm.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zcr.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wrl.cdnleiting.top

[Q15] 查询全部
来源：http://adl.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://vxw.yj20258888.top

[Q16] 查询指定列
来源：http://tll.tarul.cn

SELECT id, name FROM users;
来源：http://lsl.jinghuilouyu.cn

[Q17] 条件查询
来源：http://azx.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hlt.ybcxt.top

[Q18] 模糊匹配
来源：http://yww.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://joa.quarkkingdee.top

[Q19] 范围查询
来源：http://khv.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://afe.nwbrower.top

[Q20] IN 列表
来源：http://yfu.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lid.jyoumei.cn

[Q21] 空值判断
来源：http://ivk.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pmp.fanxiaobao.xyz

[Q22] 排序
来源：http://tmf.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gyc.fzhhl.top

[Q23] 分页
来源：http://xti.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhw.cashguo.top

[Q24] 去重
来源：http://fbz.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://chx.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://sco.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ipa.smart0.xyz

[Q26] 计数
来源：http://efc.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://lut.c1oappe.top

[Q27] 条件计数
来源：http://cum.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xae.snrcjt.cn

[Q28] 求和与平均
来源：http://sxb.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wjy.smart0.xyz

[Q29] 最大最小值
来源：http://ncn.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gyi.snrcjt.cn

[Q30] 分组统计
来源：http://ssy.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ghf.gogol.net.cn

[Q31] 分组后过滤
来源：http://vzm.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nrv.birdmap.top

[Q32] 分组拼接字符串
来源：http://ons.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xtc.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vuj.cashguo.top

[Q33] 多列分组
来源：http://xbo.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ylz.hammf.cn

[Q34] 每组取第一条
来源：http://cyy.yfazqb.com

SELECT * FROM (
来源：http://gnh.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ntj.fehbvm.com

) t WHERE rn = 1;
来源：http://yth.zhixingplan.top

[Q35] 内连接
来源：http://ssr.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kuz.wangshuangyany.cn

[Q36] 左连接
来源：http://sfl.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixh.smart0.xyz

[Q37] 右连接
来源：http://wyj.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zsl.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ioc.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jnc.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://nbb.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kai.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://khk.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tnd.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ucp.cqqwz.cn

[Q41] 多表连接
来源：http://ykq.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://huo.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://sbl.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://vvi.meibo888.top

[Q42] 连接条件附加过滤
来源：http://taz.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://yfh.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nxb.bbcook.cn

[Q43] 标量子查询
来源：http://ylf.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yni.jinqigufen.top

[Q44] IN 子查询
来源：http://rvb.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jni.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://jeg.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tnu.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://aeb.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jic.jiagoushi.top

[Q47] 与平均值比较
来源：http://ckh.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://khs.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://uef.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://irb.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://cbt.smart0.xyz

[Q49] 更新单行
来源：http://vxa.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ort.0kj1m.cn

[Q50] 批量更新
来源：http://kdw.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tqm.fehbvm.com

[Q51] 用子查询更新
来源：http://zhn.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wga.shzxlz.cn

[Q52] 删除指定行
来源：http://sfb.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://hhn.guannengcc.top

[Q53] 按条件删除
来源：http://lle.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dfv.smart0.xyz

[Q54] 清空表
来源：http://trn.epnwcf.com

TRUNCATE TABLE logs;
来源：http://kao.xuanzx.com

[Q55] 排名（并列占位）
来源：http://nij.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://suw.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://amz.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nfd.hesvh.cn

[Q57] 行号
来源：http://zcv.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eaa.yonumen.top

[Q58] 累计求和
来源：http://vyt.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ege.dianchejie.cn

[Q59] 分组内累计
来源：http://iqi.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yxw.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://qqe.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://equ.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uni.sysykeji.top

[Q61] 移动平均
来源：http://qht.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kqe.jqgfzy.top

[Q62] 分组占比
来源：http://qsw.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tcq.sysykeji.top

[Q63] 开启事务
来源：http://ufc.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://twa.xuetiantiany.cn

[Q64] 提交事务
来源：http://qhq.andypj.xyz

COMMIT;
来源：http://vvc.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://umt.xingfuxueyuan.xyz

ROLLBACK;
来源：http://cnt.havefunace.top

[Q66] 行锁查询
来源：http://qwh.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mxd.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://opg.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://onw.jinqigfzy.top

[Q68] 保存点
来源：http://coy.chenzaomai.com

SAVEPOINT sp1;
来源：http://lzd.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://dwv.yj202588.top

[Q69] 查看执行计划
来源：http://vlu.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ohb.ybcxt.top

[Q70] 更新统计信息
来源：http://ogo.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://cht.zhongyouzk.top

[Q71] 查看建表语句
来源：http://grp.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sxj.hesvh.cn

[Q72] 查看索引
来源：http://bpa.tianlin.xyz

SHOW INDEX FROM users;
来源：http://izl.jlsjyb.cn

[Q73] 查看表状态
来源：http://aax.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://sso.yuxming.cn

[Q74] 强制使用索引
来源：http://nln.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://epg.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://ebg.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xys.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mhg.jinghuilouyu.cn

[Q76] 按天统计
来源：http://zeh.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xva.9152youxi.cn

[Q77] 时间加减
来源：http://kaf.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://etg.dianchejie.cn

[Q78] 当前时间
来源：http://lwu.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bxi.sysykeji.top

[Q79] 字符串拼接
来源：http://qbv.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kye.guannengcc.top

[Q80] 字符串截取
来源：http://sbk.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zaw.tian-w.cn

[Q81] 字符串替换
来源：http://ubi.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://req.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://bzd.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hlt.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://nil.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wre.chenlongwang.top

[Q84] 去除首尾空格
来源：http://gjg.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://ddg.sweek.top

[Q85] 数值取整
来源：http://yto.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://quj.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://ddw.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gcf.cucudq.cn

[Q87] JSON 字段做条件
来源：http://vpz.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cwu.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://ygv.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wgh.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eyf.hnqzz.top

[Q89] 判断表是否存在
来源：http://ayl.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tcc.zhoulong.xyz

[Q90] 生成序号列
来源：http://erd.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mqg.daria6918.cn

================================================================================
来源：http://nws.sweek.top

R. Bash 专题
来源：http://leb.havefunace.top

================================================================================
来源：http://gdd.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://jpy.daxiang520.top

#!/usr/bin/env bash
来源：http://ujx.yj20258.top

set -euo pipefail
来源：http://xuh.fengsongda.top

[R02] 变量赋值与使用
来源：http://adh.ehwqpu.com

name="Tom"; echo "$name"
来源：http://oyp.meibo888.top

[R03] 只读变量
来源：http://bdi.vqdsnc.cn

readonly PI=3.14
来源：http://zgl.xinyue.icu

[R04] 位置参数
来源：http://lzx.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wwm.tanke756.top

[R05] 参数默认值
来源：http://sks.epnwcf.com

name="${1:-default}"
来源：http://bss.yueranfly.top

[R06] 判断命令是否存在
来源：http://dbz.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://quf.yj202588.top

[R07] if 判断文件
来源：http://rea.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zdf.fanxiaobao.xyz

[R08] 数值比较
来源：http://dro.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aga.yuanzhike.top

[R09] 字符串比较
来源：http://ita.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pjf.fanxiaobao.xyz

[R10] 正则匹配
来源：http://bfa.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cqv.yonumen.top

[R11] case 多分支
来源：http://gkb.zhoulong.xyz

case "$1" in
来源：http://dow.316326.xyz

start) echo "启动" ;;
来源：http://vht.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://rau.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://ogz.gotoacloud.top

esac
来源：http://mym.hongshengwenyu.top

[R12] for 遍历文件
来源：http://xia.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://pmb.9152youxi.cn

[R13] for 计数循环
来源：http://arp.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://zgo.havefunace.top

[R14] C 风格 for
来源：http://rtg.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sob.zdbjq.cn

[R15] while 逐行读文件
来源：http://lcn.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://idu.andypj.xyz

[R16] until 等待条件
来源：http://cen.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://big.9152youxi.cn

[R17] 数组定义与取值
来源：http://zbt.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://mpu.jlsjyb.cn

[R18] 遍历数组
来源：http://nav.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mnj.zdbjq.cn

[R19] 数组长度
来源：http://amr.9152youxi.cn

echo "${#arr[@]}"
来源：http://rsf.316326.xyz

[R20] 关联数组（字典）
来源：http://rtj.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://atl.haohaochexian.top

[R21] 字符串长度
来源：http://eno.haohaochexian.top

echo "${#s}"
来源：http://pmd.jinqigufen.top

[R22] 截取子串
来源：http://pty.hnxiangtu.top

echo "${s:0:5}"
来源：http://vwg.gzhubu.top

[R23] 字符串替换
来源：http://myw.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://thm.yongpay.top

[R24] 大小写转换
来源：http://wyp.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uvb.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://wzb.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lbd.pycfn.com

[R26] 命令替换
来源：http://qen.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://rcx.andypj.xyz

[R27] 算术展开
来源：http://wwl.cashguo.top

echo $((1 + 2 * 3))
来源：http://fjd.xziqi.cn

[R28] 浮点运算
来源：http://fbr.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://iwk.jinyuanbaomall.cn

[R29] 定义函数
来源：http://fls.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wer.gotoacloud.top

[R30] 函数返回状态码
来源：http://rti.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://srs.yfazqb.com

[R31] 局部变量
来源：http://ubu.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://owk.feifeiyinyue.top

[R32] 参数个数校验
来源：http://kug.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://err.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://dnv.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fgu.snrcjt.cn

[R34] 退出时清理
来源：http://heh.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://iie.kuanghao11.cn

[R35] 后台执行并等待
来源：http://fkk.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xnl.cucudq.cn

[R36] 并发执行多个任务
来源：http://blk.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://svb.dashuyun.cn

[R37] 把输出赋给变量
来源：http://wwk.daria6918.cn

files=$(ls -1)
来源：http://vkb.vehdjk.com

[R38] 管道串联
来源：http://yir.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://zlg.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://ilv.bbcook.cn

cmd > out.log 2>&1
来源：http://inc.yangfankeji.com

[R40] 追加写日志
来源：http://wyr.hnqzz.top

echo "log" >> out.log
来源：http://tic.zdqjudy.top

[R41] 丢弃输出
来源：http://euv.bjfxy.top

cmd >/dev/null 2>&1
来源：http://obo.jiagoushi.top

[R42] 输入重定向
来源：http://nyp.hcnkem.com

wc -l < a.txt
来源：http://htx.andypj.xyz

[R43] 按名字查找文件
来源：http://kta.hnxiangtu.top

find . -name "*.log" -type f
来源：http://rfj.316326.xyz

[R44] 按修改时间查找
来源：http://hjl.guowangkeji.top

find . -mtime -7 -type f
来源：http://rts.hesvh.cn

[R45] 批量删除
来源：http://fgx.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://emz.meibo888.top

[R46] 递归替换文件内容
来源：http://pqf.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://niq.hnqzz.top

[R47] sed 单行替换
来源：http://ojr.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://hhy.yj202588.top

[R48] awk 取指定列
来源：http://hxr.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://rnt.hesvh.cn

[R49] awk 带条件
来源：http://rga.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ekj.hammf.cn

[R50] awk 求和
来源：http://amz.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://vbh.sysykeji.top

[R51] 排序去重取前几
来源：http://heo.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jzz.sxryk.cn

[R52] 统计行数
来源：http://kge.quarkkingdee.top

wc -l a.txt
来源：http://mug.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://pzo.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://phf.jinqigufen.top

[R54] 比较两个文件
来源：http://eml.zhoulong.xyz

diff a.txt b.txt
来源：http://wib.yanxiufei.cn

[R55] 压缩与解压
来源：http://pch.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://owa.mhx1999.top

[R56] 远程拷贝
来源：http://fqq.quarkkingdee.top

scp file user@host:/path/
来源：http://soi.jqgufenzy.top

[R57] 远程执行命令
来源：http://zuu.0kj1m.cn

ssh user@host 'uptime'
来源：http://etv.jinghuilouyu.cn

[R58] 下载文件
来源：http://cjj.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mfn.ydjk.org.cn

[R59] 发 POST JSON
来源：http://wiu.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tar.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://mrg.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ojh.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://kze.ehwqpu.com


<!-- 参考信息 -->