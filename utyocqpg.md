代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iaw.smart0.xyz

[Q11] 一次插入多行
来源：http://qzi.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rsq.cheryme.top

[Q12] 插入后取自增 ID
来源：http://fzr.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cef.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://phe.bbcook.cn

[Q13] 忽略重复插入
来源：http://ung.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lno.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://nld.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gab.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mwt.zhiwuduotai.top

[Q15] 查询全部
来源：http://hwv.tian-w.cn

SELECT * FROM users;
来源：http://gaf.aizwys.cn

[Q16] 查询指定列
来源：http://vpg.52xcode.cn

SELECT id, name FROM users;
来源：http://qvx.tanke756.top

[Q17] 条件查询
来源：http://iki.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hgc.cqqwz.cn

[Q18] 模糊匹配
来源：http://rkj.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aej.andypj.xyz

[Q19] 范围查询
来源：http://qbh.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nwz.vqdsnc.cn

[Q20] IN 列表
来源：http://nim.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cht.hywenlv.cn

[Q21] 空值判断
来源：http://ord.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ztv.hysaishi.cn

[Q22] 排序
来源：http://rgn.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tff.xingfuxueyuan.xyz

[Q23] 分页
来源：http://jzh.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jjz.haohaochexian.top

[Q24] 去重
来源：http://xxh.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://yrf.52xcode.cn

[Q25] 只取前 N 条
来源：http://mfg.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cvr.xylfe.cn

[Q26] 计数
来源：http://jme.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://asg.hywenlv.cn

[Q27] 条件计数
来源：http://jgc.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dig.cdnleiting.top

[Q28] 求和与平均
来源：http://odc.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tvx.yangfankeji.com

[Q29] 最大最小值
来源：http://tnu.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cki.aizwys.cn

[Q30] 分组统计
来源：http://qji.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gfv.bbcook.cn

[Q31] 分组后过滤
来源：http://sph.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fsb.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://foa.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nvy.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rtx.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://shz.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ncl.daxiang520.top

[Q34] 每组取第一条
来源：http://atx.hongshengwenyu.top

SELECT * FROM (
来源：http://vmz.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jny.yuanzhike.top

) t WHERE rn = 1;
来源：http://tiq.nwbrower.top

[Q35] 内连接
来源：http://ytc.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ncd.nanxuanxn.top

[Q36] 左连接
来源：http://suo.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://abq.shuidangran.top

[Q37] 右连接
来源：http://bdp.meibo888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://puh.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://djb.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kjf.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://uxs.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gqk.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nja.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ukd.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wwh.smart0.xyz

[Q41] 多表连接
来源：http://eaw.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mre.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://zcs.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://dtt.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://uva.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://gre.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rbv.0kj1m.cn

[Q43] 标量子查询
来源：http://igq.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://whn.tian-w.cn

[Q44] IN 子查询
来源：http://uii.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qbe.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://awj.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhd.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://vbi.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ayt.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://wzm.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sqp.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://qyk.xinyue.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kjh.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://fwn.hongshengwenyu.top

[Q49] 更新单行
来源：http://ngg.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ysl.pengpengdd.cyou

[Q50] 批量更新
来源：http://nme.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wfv.haohaochexian.top

[Q51] 用子查询更新
来源：http://zuo.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cgq.cqqwz.cn

[Q52] 删除指定行
来源：http://gnp.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://hug.yuanzhike.top

[Q53] 按条件删除
来源：http://syc.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dfu.yj202588.top

[Q54] 清空表
来源：http://hta.andypj.xyz

TRUNCATE TABLE logs;
来源：http://jed.yj202588.top

[Q55] 排名（并列占位）
来源：http://mdg.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wta.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://mwa.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zmf.sysykeji.top

[Q57] 行号
来源：http://tbu.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zfu.pengpengdd.cyou

[Q58] 累计求和
来源：http://okt.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://art.uphjek.com

[Q59] 分组内累计
来源：http://vcl.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://arq.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://igp.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nuo.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://izk.chenlongwang.top

[Q61] 移动平均
来源：http://oow.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cuq.xuetiantiany.cn

[Q62] 分组占比
来源：http://vqo.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://arj.iojbl.cn

[Q63] 开启事务
来源：http://dme.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xyk.ehwqpu.com

[Q64] 提交事务
来源：http://try.yanxiufei.cn

COMMIT;
来源：http://lrz.tian-w.cn

[Q65] 回滚事务
来源：http://pnr.yongpay.top

ROLLBACK;
来源：http://cco.smart0.xyz

[Q66] 行锁查询
来源：http://uir.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rup.shuidangran.top

[Q67] 设置隔离级别
来源：http://srr.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdm.sjlbkw.cn

[Q68] 保存点
来源：http://zba.daria6918.cn

SAVEPOINT sp1;
来源：http://frt.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://ick.aibaodan.cn

[Q69] 查看执行计划
来源：http://kvi.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lqp.tianlin.xyz

[Q70] 更新统计信息
来源：http://xfx.nanxuanxn.top

ANALYZE TABLE users;
来源：http://cwz.daria6918.cn

[Q71] 查看建表语句
来源：http://gij.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mpl.jinqigfzy.top

[Q72] 查看索引
来源：http://hdd.nwbrower.top

SHOW INDEX FROM users;
来源：http://zoj.fehbvm.com

[Q73] 查看表状态
来源：http://lcu.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xtk.yvedp.cn

[Q74] 强制使用索引
来源：http://wlx.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mmz.pycfn.com

[Q75] 日期格式化
来源：http://lam.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gal.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uki.pycfn.com

[Q76] 按天统计
来源：http://nmp.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://azs.jianghu66.top

[Q77] 时间加减
来源：http://ihq.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fji.zhoulong.xyz

[Q78] 当前时间
来源：http://pba.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://isv.jlsjyb.cn

[Q79] 字符串拼接
来源：http://pbq.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wka.cucudq.cn

[Q80] 字符串截取
来源：http://iof.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fux.ehwqpu.com

[Q81] 字符串替换
来源：http://grg.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://psc.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://frs.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uht.cdnleiting.top

[Q83] 大小写转换
来源：http://pxz.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zpm.zycfv.cn

[Q84] 去除首尾空格
来源：http://yxd.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://ruq.bbcook.cn

[Q85] 数值取整
来源：http://sfx.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bby.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://rlg.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aer.jianghu66.top

[Q87] JSON 字段做条件
来源：http://hlj.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pah.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://siv.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lyc.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qxw.guannengcc.top

[Q89] 判断表是否存在
来源：http://ofj.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nxa.jinqigfzy.top

[Q90] 生成序号列
来源：http://ffl.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eja.bbcook.cn

================================================================================
来源：http://lei.fehbvm.com

R. Bash 专题
来源：http://eja.aizwys.cn

================================================================================
来源：http://muw.9152youxi.cn

[R01] shebang 与严格模式
来源：http://bsm.chenzaomai.com

#!/usr/bin/env bash
来源：http://thi.birdmap.top

set -euo pipefail
来源：http://dnd.ybcxt.top

[R02] 变量赋值与使用
来源：http://qnw.gogol.net.cn

name="Tom"; echo "$name"
来源：http://tno.cheryme.top

[R03] 只读变量
来源：http://oyi.kuanghao11.cn

readonly PI=3.14
来源：http://eco.yfazqb.com

[R04] 位置参数
来源：http://wwm.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nsd.bjfxy.top

[R05] 参数默认值
来源：http://alm.hammf.cn

name="${1:-default}"
来源：http://xoj.vehdjk.com

[R06] 判断命令是否存在
来源：http://ixl.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jve.shuidangran.top

[R07] if 判断文件
来源：http://jal.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://skc.daria6918.cn

[R08] 数值比较
来源：http://vvm.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rtt.zdbjq.cn

[R09] 字符串比较
来源：http://yyg.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ute.daxiang520.top

[R10] 正则匹配
来源：http://gjs.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gst.aizwys.cn

[R11] case 多分支
来源：http://rbg.shanyushiyangkeji.top

case "$1" in
来源：http://ysg.zhoulong.xyz

start) echo "启动" ;;
来源：http://dtk.zhixingplan.top

stop)  echo "停止" ;;
来源：http://xhf.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://twt.ctjpmb.com

esac
来源：http://vna.chenzaomai.com

[R12] for 遍历文件
来源：http://xfy.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://sel.hnqzz.top

[R13] for 计数循环
来源：http://aks.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://djj.ybcxt.top

[R14] C 风格 for
来源：http://tmc.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rom.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://msf.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bmn.xinyue.icu

[R16] until 等待条件
来源：http://vek.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xnc.zhongyouzk.top

[R17] 数组定义与取值
来源：http://omu.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://qaq.zhijiandao.cn

[R18] 遍历数组
来源：http://meq.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ccj.hfpthk.cn

[R19] 数组长度
来源：http://uuh.guowangkeji.top

echo "${#arr[@]}"
来源：http://isw.snrcjt.cn

[R20] 关联数组（字典）
来源：http://cxa.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mnt.hysaishi.cn

[R21] 字符串长度
来源：http://cjs.316326.xyz

echo "${#s}"
来源：http://apm.cqqwz.cn

[R22] 截取子串
来源：http://ohj.xziqi.cn

echo "${s:0:5}"
来源：http://dqf.hongshengwenyu.top

[R23] 字符串替换
来源：http://eeu.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rgn.jyoumei.cn

[R24] 大小写转换
来源：http://rku.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lms.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://zbx.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://mkk.vehdjk.com

[R26] 命令替换
来源：http://xby.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://mzc.cashguo.top

[R27] 算术展开
来源：http://ymn.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://haw.hnqzz.top

[R28] 浮点运算
来源：http://bbg.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://yfp.hongshengwenyu.top

[R29] 定义函数
来源：http://fur.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://srt.cdnleiting.top

[R30] 函数返回状态码
来源：http://zua.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://lri.pycfn.com

[R31] 局部变量
来源：http://fyl.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://tam.gotoacloud.top

[R32] 参数个数校验
来源：http://ila.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oxx.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://dbi.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oxo.yueranfly.top

[R34] 退出时清理
来源：http://bcx.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jgr.epnwcf.com

[R35] 后台执行并等待
来源：http://iss.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lwq.shzxlz.cn

[R36] 并发执行多个任务
来源：http://hve.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ush.havefunace.top

[R37] 把输出赋给变量
来源：http://pxw.dashuyun.cn

files=$(ls -1)
来源：http://opx.wangdashe.top

[R38] 管道串联
来源：http://xfm.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://yhd.cheryme.top

[R39] 重定向标准输出与错误
来源：http://gxh.meibo888.top

cmd > out.log 2>&1
来源：http://mqv.cqqwz.cn

[R40] 追加写日志
来源：http://cad.ehwqpu.com

echo "log" >> out.log
来源：http://pwa.shangyingyoupin.top

[R41] 丢弃输出
来源：http://yzs.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://xbv.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://mwl.shzxlz.cn

wc -l < a.txt
来源：http://nex.smart0.xyz

[R43] 按名字查找文件
来源：http://pzv.hnqzz.top

find . -name "*.log" -type f
来源：http://qpw.hcnkem.com

[R44] 按修改时间查找
来源：http://djn.hesvh.cn

find . -mtime -7 -type f
来源：http://lew.shanyushiyangkeji.top

[R45] 批量删除
来源：http://eoy.guannengcc.top

find . -name "*.tmp" -delete
来源：http://gar.yangfankeji.com

[R46] 递归替换文件内容
来源：http://ffp.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bcj.xuanzx.com

[R47] sed 单行替换
来源：http://clk.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fuf.yfazqb.com

[R48] awk 取指定列
来源：http://hjl.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://ira.cdnleiting.top

[R49] awk 带条件
来源：http://pjl.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kzw.zycfv.cn

[R50] awk 求和
来源：http://ztg.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://gpl.nanxinkj.top

[R51] 排序去重取前几
来源：http://ggj.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iff.hnxiangtu.top

[R52] 统计行数
来源：http://vmn.hnqzz.top

wc -l a.txt
来源：http://kgb.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://ols.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://myo.jianghu66.top

[R54] 比较两个文件
来源：http://kah.yj20258888.top

diff a.txt b.txt
来源：http://ovt.52xcode.cn

[R55] 压缩与解压
来源：http://xng.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wch.jqgufenzy.top

[R56] 远程拷贝
来源：http://uzn.316326.xyz

scp file user@host:/path/
来源：http://cbk.yonumen.top

[R57] 远程执行命令
来源：http://nsp.hcnkem.com

ssh user@host 'uptime'
来源：http://jig.fktsv.cn

[R58] 下载文件
来源：http://vkh.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ynm.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://rlg.ybcxt.top


<!-- 参考信息 -->