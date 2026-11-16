代发 wailian999

SELECT * FROM users;
来源：http://ent.dianchejie.cn

[Q16] 查询指定列
来源：http://lwy.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://qpx.epnwcf.com

[Q17] 条件查询
来源：http://kgd.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ugv.chenlongwang.top

[Q18] 模糊匹配
来源：http://rhr.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hmm.havefunace.top

[Q19] 范围查询
来源：http://hjg.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jbj.wangshuangyany.cn

[Q20] IN 列表
来源：http://bak.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ggb.cucudq.cn

[Q21] 空值判断
来源：http://rti.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qsw.ybcxt.top

[Q22] 排序
来源：http://eca.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zwy.cqqwz.cn

[Q23] 分页
来源：http://lin.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zam.xylfe.cn

[Q24] 去重
来源：http://mfb.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://rht.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://oyc.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wos.gogol.net.cn

[Q26] 计数
来源：http://hqu.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://pfl.meibo888.top

[Q27] 条件计数
来源：http://rvw.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eom.fehbvm.com

[Q28] 求和与平均
来源：http://mad.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zfh.hnxiangtu.top

[Q29] 最大最小值
来源：http://olz.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vsu.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://ymv.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hms.cashguo.top

[Q31] 分组后过滤
来源：http://ecv.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ske.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://unp.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qtf.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lsc.zhiwuduotai.top

[Q33] 多列分组
来源：http://vtv.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://avi.tian-w.cn

[Q34] 每组取第一条
来源：http://dve.shanyushiyangtech.top

SELECT * FROM (
来源：http://hgp.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gjg.iojbl.cn

) t WHERE rn = 1;
来源：http://gnl.zhijiandao.cn

[Q35] 内连接
来源：http://jya.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bkk.xuetiantiany.cn

[Q36] 左连接
来源：http://cqi.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ecc.yj20258888.top

[Q37] 右连接
来源：http://scl.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xhl.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://weu.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dfo.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://kit.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tyc.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://raw.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fgi.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xfk.cheryme.top

[Q41] 多表连接
来源：http://ood.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lkt.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://ala.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://yfp.cheryme.top

[Q42] 连接条件附加过滤
来源：http://dkw.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://bqn.sjlbkw.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://crr.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://hho.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rbn.mhx1999.top

[Q44] IN 子查询
来源：http://ndh.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bjp.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://rxz.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wjt.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://dnt.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://btk.xinyue.icu

[Q47] 与平均值比较
来源：http://anf.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cvv.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://slz.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rwz.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://xoa.nanxuanxn.top

[Q49] 更新单行
来源：http://gmt.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nys.zhoulong.xyz

[Q50] 批量更新
来源：http://tiw.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lsb.chenzaomai.com

[Q51] 用子查询更新
来源：http://occ.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ouy.tianlin.xyz

[Q52] 删除指定行
来源：http://tdc.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://jjj.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://yjb.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://okc.0kj1m.cn

[Q54] 清空表
来源：http://cha.yueranfly.top

TRUNCATE TABLE logs;
来源：http://gxq.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://pvs.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://agm.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://dlj.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ghl.sweek.top

[Q57] 行号
来源：http://ain.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://meo.xuanzx.com

[Q58] 累计求和
来源：http://emw.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yvh.yfazqb.com

[Q59] 分组内累计
来源：http://xlb.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qnj.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://kbe.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wnq.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wiu.tanke756.top

[Q61] 移动平均
来源：http://ugj.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://egk.quarkkingdee.top

[Q62] 分组占比
来源：http://vhx.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fdn.dashuyun.cn

[Q63] 开启事务
来源：http://ztg.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nzj.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://jfj.jinqigfzy.top

COMMIT;
来源：http://daa.yanxiufei.cn

[Q65] 回滚事务
来源：http://zgt.chenzaomai.com

ROLLBACK;
来源：http://rov.xuanzx.com

[Q66] 行锁查询
来源：http://ekg.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uao.gotoacloud.top

[Q67] 设置隔离级别
来源：http://uct.daria6918.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://doz.daxiang520.top

[Q68] 保存点
来源：http://asg.bjfxy.top

SAVEPOINT sp1;
来源：http://wzh.zycfv.cn

ROLLBACK TO sp1;
来源：http://bxj.yangfankeji.com

[Q69] 查看执行计划
来源：http://tda.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ojw.0kj1m.cn

[Q70] 更新统计信息
来源：http://vvt.52xcode.cn

ANALYZE TABLE users;
来源：http://fxj.daxiang520.top

[Q71] 查看建表语句
来源：http://lgd.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yet.ppjwa.cn

[Q72] 查看索引
来源：http://pul.shzxlz.cn

SHOW INDEX FROM users;
来源：http://bts.ybcxt.top

[Q73] 查看表状态
来源：http://xkp.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://cfb.jiagoushi.top

[Q74] 强制使用索引
来源：http://txg.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rqy.tian-w.cn

[Q75] 日期格式化
来源：http://lva.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lmw.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cge.iojbl.cn

[Q76] 按天统计
来源：http://rut.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uix.guowangkeji.top

[Q77] 时间加减
来源：http://jam.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fob.chenjidiqi.icu

[Q78] 当前时间
来源：http://rek.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rdx.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://bnd.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xmc.daria6918.cn

[Q80] 字符串截取
来源：http://moh.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dui.jlsjyb.cn

[Q81] 字符串替换
来源：http://obt.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hmc.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://qfg.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kaz.gogol.net.cn

[Q83] 大小写转换
来源：http://ofu.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://upg.daxiang520.top

[Q84] 去除首尾空格
来源：http://jpv.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://zpm.fehbvm.com

[Q85] 数值取整
来源：http://pzm.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fzq.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://kks.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zxr.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://gld.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kha.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://ung.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fdp.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bfc.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://ksa.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yiy.redwolf501.top

[Q90] 生成序号列
来源：http://aal.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mnc.ydjk.org.cn

================================================================================
来源：http://eco.gzhubu.top

R. Bash 专题
来源：http://ngw.snrcjt.cn

================================================================================
来源：http://ghj.52xcode.cn

[R01] shebang 与严格模式
来源：http://nvg.shuidangran.top

#!/usr/bin/env bash
来源：http://rwc.gzhubu.top

set -euo pipefail
来源：http://srj.hammf.cn

[R02] 变量赋值与使用
来源：http://iju.zhixingplan.top

name="Tom"; echo "$name"
来源：http://jqm.yvedp.cn

[R03] 只读变量
来源：http://ctd.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://uol.sysykeji.top

[R04] 位置参数
来源：http://kpt.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yid.tianlin.xyz

[R05] 参数默认值
来源：http://nie.pengpengdd.cyou

name="${1:-default}"
来源：http://drg.pycfn.com

[R06] 判断命令是否存在
来源：http://fqo.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://evc.0kj1m.cn

[R07] if 判断文件
来源：http://knm.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zlp.cashguo.top

[R08] 数值比较
来源：http://pem.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://utf.xziqi.cn

[R09] 字符串比较
来源：http://sng.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqe.ctjpmb.com

[R10] 正则匹配
来源：http://vdk.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ttk.0kj1m.cn

[R11] case 多分支
来源：http://lgy.smart0.xyz

case "$1" in
来源：http://hvn.ctjpmb.com

start) echo "启动" ;;
来源：http://dmf.yj20258.top

stop)  echo "停止" ;;
来源：http://xqt.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://jds.yfazqb.com

esac
来源：http://dti.xziqi.cn

[R12] for 遍历文件
来源：http://mee.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://uid.aizwys.cn

[R13] for 计数循环
来源：http://mvu.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://ikc.jqgfzy.top

[R14] C 风格 for
来源：http://mkd.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mqw.sjlbkw.cn

[R15] while 逐行读文件
来源：http://wsa.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lrp.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://tsp.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uhk.ppjwa.cn

[R17] 数组定义与取值
来源：http://kjd.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vua.uphjek.com

[R18] 遍历数组
来源：http://xgg.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oqy.zdqjudy.top

[R19] 数组长度
来源：http://djy.zhoulong.xyz

echo "${#arr[@]}"
来源：http://lvc.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://apd.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dgo.ehwqpu.com

[R21] 字符串长度
来源：http://aaq.tian-w.cn

echo "${#s}"
来源：http://hhv.cashguo.top

[R22] 截取子串
来源：http://ipa.redwolf501.top

echo "${s:0:5}"
来源：http://uqm.gzhubu.top

[R23] 字符串替换
来源：http://tao.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bol.shanyushiyangtech.top

[R24] 大小写转换
来源：http://pnk.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://rbp.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://hun.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dtr.sjlbkw.cn

[R26] 命令替换
来源：http://tim.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://zuv.ywan-chungtsiang.top

[R27] 算术展开
来源：http://kah.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://ira.daxiang520.top

[R28] 浮点运算
来源：http://fcy.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://qaa.yueranfly.top

[R29] 定义函数
来源：http://eze.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yxe.meibo888.top

[R30] 函数返回状态码
来源：http://jlo.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://mnr.sufxvd.cn

[R31] 局部变量
来源：http://kit.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://cao.zhixingplan.top

[R32] 参数个数校验
来源：http://ezl.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lwl.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://iou.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kup.daxiang520.top

[R34] 退出时清理
来源：http://tzo.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://kfj.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://kfl.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yyz.epnwcf.com

[R36] 并发执行多个任务
来源：http://nle.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://byr.aizwys.cn

[R37] 把输出赋给变量
来源：http://btk.daria6918.cn

files=$(ls -1)
来源：http://wle.xinyue.icu

[R38] 管道串联
来源：http://vbz.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://hkf.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://lam.bjfxy.top

cmd > out.log 2>&1
来源：http://bbz.shanyushiyangtech.top

[R40] 追加写日志
来源：http://hpv.vehdjk.com

echo "log" >> out.log
来源：http://adg.hcnkem.com

[R41] 丢弃输出
来源：http://rxn.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://oyu.pengpengdd.cyou

[R42] 输入重定向
来源：http://ktn.sweek.top

wc -l < a.txt
来源：http://fnx.zdbjq.cn

[R43] 按名字查找文件
来源：http://otu.yueranfly.top

find . -name "*.log" -type f
来源：http://vlt.ehwqpu.com

[R44] 按修改时间查找
来源：http://tjf.jinqigfzy.top

find . -mtime -7 -type f
来源：http://qok.chenlongwang.top

[R45] 批量删除
来源：http://rmd.smart0.xyz

find . -name "*.tmp" -delete
来源：http://zwd.yj20258.top

[R46] 递归替换文件内容
来源：http://yjv.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hpb.ehwqpu.com

[R47] sed 单行替换
来源：http://yrl.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://qzp.chenjidiqi.icu

[R48] awk 取指定列
来源：http://uak.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://xeg.havefunace.top

[R49] awk 带条件
来源：http://dpt.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iow.snrcjt.cn

[R50] awk 求和
来源：http://tfe.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://say.sysykeji.top

[R51] 排序去重取前几
来源：http://cof.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ccy.cdnleiting.top

[R52] 统计行数
来源：http://cbh.yj202588.top

wc -l a.txt
来源：http://xhh.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://qdx.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uii.pycfn.com

[R54] 比较两个文件
来源：http://ueu.gogol.net.cn

diff a.txt b.txt
来源：http://lue.nanxinkj.top

[R55] 压缩与解压
来源：http://kek.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://two.feifeiyinyue.top

[R56] 远程拷贝
来源：http://uwk.zdqjudy.top

scp file user@host:/path/
来源：http://xek.redwolf501.top

[R57] 远程执行命令
来源：http://xea.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://xot.xziqi.cn

[R58] 下载文件
来源：http://lgb.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xfo.ivvv.top

[R59] 发 POST JSON
来源：http://kdw.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ixf.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://hxw.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jki.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://miq.hnxiangtu.top

df -h;  du -sh *
来源：http://jro.vehdjk.com

[R62] 找最占空间的文件
来源：http://cyq.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://nns.hammf.cn

[R63] 内存与进程
来源：http://wry.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://vhm.fengsongda.top

[R64] 结束进程
来源：http://tqj.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://aic.haohaochexian.top

[R65] 查看端口占用
来源：http://cvz.xziqi.cn


<!-- 参考信息 -->