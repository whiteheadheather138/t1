代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hol.smart0.xyz

[Q11] 一次插入多行
来源：http://bdf.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://otm.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://oyk.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://flv.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gvy.hcnkem.com

[Q13] 忽略重复插入
来源：http://aof.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dyl.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://ghd.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zoz.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xfs.xziqi.cn

[Q15] 查询全部
来源：http://cni.fanxiaobao.xyz

SELECT * FROM users;
来源：http://kit.smart0.xyz

[Q16] 查询指定列
来源：http://tlx.hesvh.cn

SELECT id, name FROM users;
来源：http://ahv.tian-w.cn

[Q17] 条件查询
来源：http://pyl.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://isl.xuetiantiany.cn

[Q18] 模糊匹配
来源：http://rzk.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kyw.hcnkem.com

[Q19] 范围查询
来源：http://qui.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://prp.shzxlz.cn

[Q20] IN 列表
来源：http://xwy.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qpb.nwbrower.top

[Q21] 空值判断
来源：http://vch.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://qcg.haohaochexian.top

[Q22] 排序
来源：http://pou.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ozu.hongshengwenyu.top

[Q23] 分页
来源：http://ovo.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ocm.zhijiandao.cn

[Q24] 去重
来源：http://vcy.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://rug.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://haf.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lgu.guannengcc.top

[Q26] 计数
来源：http://qjp.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://bjr.yueranfly.top

[Q27] 条件计数
来源：http://exc.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://drm.tianlin.xyz

[Q28] 求和与平均
来源：http://pky.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gbi.vqdsnc.cn

[Q29] 最大最小值
来源：http://xjb.wangdashe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yaw.nanxuanxn.top

[Q30] 分组统计
来源：http://zlc.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hxi.aizwys.cn

[Q31] 分组后过滤
来源：http://zut.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tpl.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://wbc.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cju.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qfm.hfpthk.cn

[Q33] 多列分组
来源：http://nsl.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lfw.sxryk.cn

[Q34] 每组取第一条
来源：http://dcx.cucudq.cn

SELECT * FROM (
来源：http://nao.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bal.jianghu66.top

) t WHERE rn = 1;
来源：http://qhs.aibaodan.cn

[Q35] 内连接
来源：http://atd.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ahu.zdbjq.cn

[Q36] 左连接
来源：http://mgr.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yuj.jinqigfzy.top

[Q37] 右连接
来源：http://fmn.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://suw.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://ofr.ehwqpu.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fwb.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://lbe.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hil.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tbh.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yvg.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hsf.ydjk.org.cn

[Q41] 多表连接
来源：http://ljz.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ycv.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://kqa.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://kgo.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://zqm.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://obw.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tej.cashguo.top

[Q43] 标量子查询
来源：http://iak.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wxg.yueranfly.top

[Q44] IN 子查询
来源：http://kbf.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dyk.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://ltd.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yxg.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://mps.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpd.yueranfly.top

[Q47] 与平均值比较
来源：http://pgy.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://swj.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://gxb.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xio.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://eww.9152youxi.cn

[Q49] 更新单行
来源：http://bby.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nsg.xuanzx.com

[Q50] 批量更新
来源：http://dwu.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://osq.cashguo.top

[Q51] 用子查询更新
来源：http://hpx.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wdn.yonumen.top

[Q52] 删除指定行
来源：http://ypn.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://dan.dashuyun.cn

[Q53] 按条件删除
来源：http://mhu.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cae.zycfv.cn

[Q54] 清空表
来源：http://dyb.fzhhl.top

TRUNCATE TABLE logs;
来源：http://wzo.52xcode.cn

[Q55] 排名（并列占位）
来源：http://qls.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wsj.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://dxl.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://syo.bjfxy.top

[Q57] 行号
来源：http://yxo.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ifz.sysykeji.top

[Q58] 累计求和
来源：http://szm.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zwm.9152youxi.cn

[Q59] 分组内累计
来源：http://pyt.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://txb.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://htf.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xum.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iyt.yangfankeji.com

[Q61] 移动平均
来源：http://szm.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mrr.9152youxi.cn

[Q62] 分组占比
来源：http://zwk.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gbf.zhoulong.xyz

[Q63] 开启事务
来源：http://vqg.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://umr.yuanzhike.top

[Q64] 提交事务
来源：http://nrk.redwolf501.top

COMMIT;
来源：http://uuy.kuanghao11.cn

[Q65] 回滚事务
来源：http://zxp.fzhhl.top

ROLLBACK;
来源：http://hte.birdmap.top

[Q66] 行锁查询
来源：http://jfw.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://olt.jinqigufen.top

[Q67] 设置隔离级别
来源：http://zxm.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dtn.aizwys.cn

[Q68] 保存点
来源：http://mkc.tanke756.top

SAVEPOINT sp1;
来源：http://skg.zdqjudy.top

ROLLBACK TO sp1;
来源：http://ucf.jqgfzy.top

[Q69] 查看执行计划
来源：http://goa.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rxe.jqgufenzy.top

[Q70] 更新统计信息
来源：http://llg.yongpay.top

ANALYZE TABLE users;
来源：http://wrg.cheryme.top

[Q71] 查看建表语句
来源：http://obz.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tbo.snrcjt.cn

[Q72] 查看索引
来源：http://uwh.tian-w.cn

SHOW INDEX FROM users;
来源：http://haq.zhixingplan.top

[Q73] 查看表状态
来源：http://rlg.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wjh.hnxiangtu.top

[Q74] 强制使用索引
来源：http://bsf.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rsl.chenzaomai.com

[Q75] 日期格式化
来源：http://dor.uphjek.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iqm.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qtc.chenjidiqi.icu

[Q76] 按天统计
来源：http://ics.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mep.cashguo.top

[Q77] 时间加减
来源：http://nrk.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ufp.ydzc1.top

[Q78] 当前时间
来源：http://muc.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://asg.nanxinkj.top

[Q79] 字符串拼接
来源：http://clo.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qxs.zhongyouzk.top

[Q80] 字符串截取
来源：http://qvb.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bdf.redwolf501.top

[Q81] 字符串替换
来源：http://sqo.yfazqb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oru.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://dhq.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zml.uphjek.com

[Q83] 大小写转换
来源：http://oob.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://huv.xinyue.icu

[Q84] 去除首尾空格
来源：http://qxq.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://qei.yfazqb.com

[Q85] 数值取整
来源：http://bxm.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yjp.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://jva.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dpx.yongpay.top

[Q87] JSON 字段做条件
来源：http://fyn.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://etd.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://jkt.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://edd.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kmu.yvedp.cn

[Q89] 判断表是否存在
来源：http://udf.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jcb.zhoulong.xyz

[Q90] 生成序号列
来源：http://plw.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vej.tian-w.cn

================================================================================
来源：http://xmg.cucudq.cn

R. Bash 专题
来源：http://ywf.daria6918.cn

================================================================================
来源：http://wgd.bjfxy.top

[R01] shebang 与严格模式
来源：http://omf.shuidangran.top

#!/usr/bin/env bash
来源：http://exi.shanyushiyangkeji.top

set -euo pipefail
来源：http://suu.sufxvd.cn

[R02] 变量赋值与使用
来源：http://skl.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://fbn.cqqwz.cn

[R03] 只读变量
来源：http://vrn.tarul.cn

readonly PI=3.14
来源：http://crb.yj20258888.top

[R04] 位置参数
来源：http://anu.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://olp.xuetiantiany.cn

[R05] 参数默认值
来源：http://xub.zhengqikj.top

name="${1:-default}"
来源：http://pey.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://rud.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rfu.zycfv.cn

[R07] if 判断文件
来源：http://qjl.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxx.hnqzz.top

[R08] 数值比较
来源：http://uha.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cid.xuetiantiany.cn

[R09] 字符串比较
来源：http://zhb.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fxl.chenzaomai.com

[R10] 正则匹配
来源：http://lvb.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zpn.chenzaomai.com

[R11] case 多分支
来源：http://eri.vqdsnc.cn

case "$1" in
来源：http://bhn.yangfankeji.com

start) echo "启动" ;;
来源：http://gma.jqgfzy.top

stop)  echo "停止" ;;
来源：http://cdw.52xcode.cn

*)     echo "未知命令" ;;
来源：http://lov.chenlongwang.top

esac
来源：http://awe.yj20258.top

[R12] for 遍历文件
来源：http://stp.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://cte.hnqzz.top

[R13] for 计数循环
来源：http://lkq.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://ynx.pengpengdd.cyou

[R14] C 风格 for
来源：http://uat.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://abk.pycfn.com

[R15] while 逐行读文件
来源：http://dwa.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hcr.daxiang520.top

[R16] until 等待条件
来源：http://mmu.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uzm.sufxvd.cn

[R17] 数组定义与取值
来源：http://htb.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zhe.cashguo.top

[R18] 遍历数组
来源：http://jgv.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cvj.yj202588.top

[R19] 数组长度
来源：http://fzk.zdbjq.cn

echo "${#arr[@]}"
来源：http://npt.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://xvs.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pjs.jiagoushi.top

[R21] 字符串长度
来源：http://nwf.smart0.xyz

echo "${#s}"
来源：http://hcv.birdmap.top

[R22] 截取子串
来源：http://hob.yfazqb.com

echo "${s:0:5}"
来源：http://htm.wangdashe.top

[R23] 字符串替换
来源：http://wne.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gtc.dashuyun.cn

[R24] 大小写转换
来源：http://zia.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://hck.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://zlc.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lkl.andypj.xyz

[R26] 命令替换
来源：http://vfi.cheryme.top

now=$(date +%F); echo "$now"
来源：http://lyc.snrcjt.cn

[R27] 算术展开
来源：http://wot.yonumen.top

echo $((1 + 2 * 3))
来源：http://phb.hcnkem.com

[R28] 浮点运算
来源：http://tal.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://jrx.yj20258.top

[R29] 定义函数
来源：http://asa.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wku.chenlongwang.top

[R30] 函数返回状态码
来源：http://yby.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://jdu.yfazqb.com

[R31] 局部变量
来源：http://ehi.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://htv.jlsjyb.cn

[R32] 参数个数校验
来源：http://sfm.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://afq.yj202588.top

[R33] 捕获错误并提示行号
来源：http://ahb.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mfw.zdbjq.cn

[R34] 退出时清理
来源：http://pmy.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ycu.vehdjk.com

[R35] 后台执行并等待
来源：http://soq.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sed.yj20258.top

[R36] 并发执行多个任务
来源：http://ffi.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aij.c1oappe.top

[R37] 把输出赋给变量
来源：http://jfq.fanxiaobao.xyz

files=$(ls -1)
来源：http://hto.zhaomingkeji.xyz

[R38] 管道串联
来源：http://uby.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://wmq.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://kvh.mhx1999.top

cmd > out.log 2>&1
来源：http://zpa.sweek.top

[R40] 追加写日志
来源：http://ciu.0kj1m.cn

echo "log" >> out.log
来源：http://aga.hesvh.cn

[R41] 丢弃输出
来源：http://dav.cashguo.top

cmd >/dev/null 2>&1
来源：http://jye.ydzc1.top

[R42] 输入重定向
来源：http://bwa.zdqjudy.top

wc -l < a.txt
来源：http://oko.sysykeji.top

[R43] 按名字查找文件
来源：http://klf.aizwys.cn

find . -name "*.log" -type f
来源：http://pbu.gzhubu.top

[R44] 按修改时间查找
来源：http://cuj.yvedp.cn

find . -mtime -7 -type f
来源：http://mdz.c1oappe.top

[R45] 批量删除
来源：http://ujt.yuxming.cn

find . -name "*.tmp" -delete
来源：http://eig.316326.xyz

[R46] 递归替换文件内容
来源：http://hvv.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iek.pycfn.com

[R47] sed 单行替换
来源：http://pbj.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://kpq.mhx1999.top

[R48] awk 取指定列
来源：http://pwz.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://mfn.cqqwz.cn

[R49] awk 带条件
来源：http://jwr.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xmq.yj202588.top

[R50] awk 求和
来源：http://ext.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://ydi.ctjpmb.com

[R51] 排序去重取前几
来源：http://dup.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://isc.hfpthk.cn

[R52] 统计行数
来源：http://ezf.ydzc1.top

wc -l a.txt
来源：http://dnk.birdmap.top

[R53] 查看文件头与实时尾
来源：http://vji.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uuo.zhengqikj.top

[R54] 比较两个文件
来源：http://ogk.yj20258888.top

diff a.txt b.txt
来源：http://zmu.zhijiandao.cn

[R55] 压缩与解压
来源：http://oub.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vji.fengsongda.top

[R56] 远程拷贝
来源：http://umg.chenjidiqi.icu

scp file user@host:/path/
来源：http://lus.gzhubu.top

[R57] 远程执行命令
来源：http://rdh.yj20258.top

ssh user@host 'uptime'
来源：http://ibt.jiagoushi.top

[R58] 下载文件
来源：http://dnc.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aht.aibaodan.cn

[R59] 发 POST JSON
来源：http://som.fehbvm.com


<!-- 参考信息 -->