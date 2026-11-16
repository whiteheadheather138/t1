代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ioo.52xcode.cn

[Q18] 模糊匹配
来源：http://zfo.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xgv.zhengqikj.top

[Q19] 范围查询
来源：http://ahn.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mqh.gotoacloud.top

[Q20] IN 列表
来源：http://uof.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kpr.hysaishi.cn

[Q21] 空值判断
来源：http://bts.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://mxc.gotoacloud.top

[Q22] 排序
来源：http://bsl.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tct.redwolf501.top

[Q23] 分页
来源：http://gds.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rgn.hfpthk.cn

[Q24] 去重
来源：http://hcw.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://vql.zhixingplan.top

[Q25] 只取前 N 条
来源：http://ivs.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://shu.guowangkeji.top

[Q26] 计数
来源：http://ncc.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://xel.ivvv.top

[Q27] 条件计数
来源：http://wwp.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gzs.wangdashe.top

[Q28] 求和与平均
来源：http://svu.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ajr.iojbl.cn

[Q29] 最大最小值
来源：http://ymt.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://imf.fehbvm.com

[Q30] 分组统计
来源：http://fkj.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://obf.shuidangran.top

[Q31] 分组后过滤
来源：http://xop.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kau.52xcode.cn

[Q32] 分组拼接字符串
来源：http://irg.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dtr.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bvp.xuanzx.com

[Q33] 多列分组
来源：http://xnt.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ggy.vehdjk.com

[Q34] 每组取第一条
来源：http://xxe.andypj.xyz

SELECT * FROM (
来源：http://ixo.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gbx.zdqjudy.top

) t WHERE rn = 1;
来源：http://baa.ivvv.top

[Q35] 内连接
来源：http://cxb.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ghs.sweek.top

[Q36] 左连接
来源：http://jgt.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://spp.epnwcf.com

[Q37] 右连接
来源：http://sbf.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://anb.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://unk.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hhw.uphjek.com

[Q39] 自连接（查上下级）
来源：http://wdn.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pwu.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pay.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ghh.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jub.zhoulong.xyz

[Q41] 多表连接
来源：http://brx.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ybj.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://wlq.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://njq.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://sdh.bbcook.cn

SELECT u.name, o.amount FROM users u
来源：http://fvs.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kaw.yonumen.top

[Q43] 标量子查询
来源：http://jdt.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://agh.epnwcf.com

[Q44] IN 子查询
来源：http://fni.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xlm.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://pjz.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pmd.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://tip.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xhu.yj20258888.top

[Q47] 与平均值比较
来源：http://ilm.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nvk.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://zes.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hdm.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://qlh.jiagoushi.top

[Q49] 更新单行
来源：http://mzl.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vlx.wangdashe.top

[Q50] 批量更新
来源：http://zal.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://crx.hfpthk.cn

[Q51] 用子查询更新
来源：http://bja.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lru.ydjk.org.cn

[Q52] 删除指定行
来源：http://vjx.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://syo.zhiwuduotai.top

[Q53] 按条件删除
来源：http://skd.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://erp.yonumen.top

[Q54] 清空表
来源：http://ysd.vehdjk.com

TRUNCATE TABLE logs;
来源：http://icd.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://glh.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tgz.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://bdk.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ovs.9152youxi.cn

[Q57] 行号
来源：http://etj.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fxw.meibo888.top

[Q58] 累计求和
来源：http://nrp.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ohr.xylfe.cn

[Q59] 分组内累计
来源：http://hiz.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://reu.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://ywx.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sqb.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jbn.fanxiaobao.xyz

[Q61] 移动平均
来源：http://usk.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uqr.hesvh.cn

[Q62] 分组占比
来源：http://nnj.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cek.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://sfy.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://xpd.hfpthk.cn

[Q64] 提交事务
来源：http://tag.yj20258.top

COMMIT;
来源：http://bqs.cucudq.cn

[Q65] 回滚事务
来源：http://afi.snrcjt.cn

ROLLBACK;
来源：http://dgz.yfazqb.com

[Q66] 行锁查询
来源：http://kew.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wtc.hnqzz.top

[Q67] 设置隔离级别
来源：http://pvm.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pym.zdqjudy.top

[Q68] 保存点
来源：http://tij.c1oappe.top

SAVEPOINT sp1;
来源：http://oqp.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://baf.shuidangran.top

[Q69] 查看执行计划
来源：http://jhq.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zkd.ydzc1.top

[Q70] 更新统计信息
来源：http://kul.hywenlv.cn

ANALYZE TABLE users;
来源：http://rsh.jqgfzy.top

[Q71] 查看建表语句
来源：http://dqj.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bko.gaohongyu789.top

[Q72] 查看索引
来源：http://nmq.daria6918.cn

SHOW INDEX FROM users;
来源：http://nys.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://bhh.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://sou.chenzaomai.com

[Q74] 强制使用索引
来源：http://aih.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rvh.chenjidiqi.icu

[Q75] 日期格式化
来源：http://yhe.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://spo.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qio.yuxming.cn

[Q76] 按天统计
来源：http://uxd.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hik.svipenyu.cn

[Q77] 时间加减
来源：http://mvh.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fzj.vehdjk.com

[Q78] 当前时间
来源：http://xsn.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qcf.gzhubu.top

[Q79] 字符串拼接
来源：http://qrz.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tbg.jinqigfzy.top

[Q80] 字符串截取
来源：http://wow.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ybu.gogol.net.cn

[Q81] 字符串替换
来源：http://wrj.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iix.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://vvj.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bon.tanke756.top

[Q83] 大小写转换
来源：http://lfx.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kij.aizwys.cn

[Q84] 去除首尾空格
来源：http://kme.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://rnj.tanke756.top

[Q85] 数值取整
来源：http://ihi.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nbo.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://xmw.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fan.jianghu66.top

[Q87] JSON 字段做条件
来源：http://rwz.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bxq.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://nly.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://crh.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wnw.tianlin.xyz

[Q89] 判断表是否存在
来源：http://wbq.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ian.gogol.net.cn

[Q90] 生成序号列
来源：http://blx.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tpp.pycfn.com

================================================================================
来源：http://cma.jinghuilouyu.cn

R. Bash 专题
来源：http://kcn.jyoumei.cn

================================================================================
来源：http://oas.ivvv.top

[R01] shebang 与严格模式
来源：http://pgs.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://jdp.ywan-chungtsiang.top

set -euo pipefail
来源：http://hyt.nwbrower.top

[R02] 变量赋值与使用
来源：http://flm.yj20258.top

name="Tom"; echo "$name"
来源：http://mle.9152youxi.cn

[R03] 只读变量
来源：http://tqa.hammf.cn

readonly PI=3.14
来源：http://dpf.316326.xyz

[R04] 位置参数
来源：http://doq.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mol.yj20258.top

[R05] 参数默认值
来源：http://gkx.jlsjyb.cn

name="${1:-default}"
来源：http://prm.mhx1999.top

[R06] 判断命令是否存在
来源：http://ftx.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ici.zhongyouzk.top

[R07] if 判断文件
来源：http://ibb.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://auq.jinghuilouyu.cn

[R08] 数值比较
来源：http://jdq.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sbr.jyoumei.cn

[R09] 字符串比较
来源：http://ajv.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://plu.haohaochexian.top

[R10] 正则匹配
来源：http://ddn.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bca.ehwqpu.com

[R11] case 多分支
来源：http://syc.tian-w.cn

case "$1" in
来源：http://pjt.feifeiyinyue.top

start) echo "启动" ;;
来源：http://jwf.yonumen.top

stop)  echo "停止" ;;
来源：http://dfp.yj202588.top

*)     echo "未知命令" ;;
来源：http://inr.daxiang520.top

esac
来源：http://utb.quarkkingdee.top

[R12] for 遍历文件
来源：http://wrt.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://lcm.0kj1m.cn

[R13] for 计数循环
来源：http://lpu.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://vpu.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://irt.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rnv.yueranfly.top

[R15] while 逐行读文件
来源：http://noa.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://njl.yangfankeji.com

[R16] until 等待条件
来源：http://qee.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nzq.ppjwa.cn

[R17] 数组定义与取值
来源：http://kyp.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vkm.redwolf501.top

[R18] 遍历数组
来源：http://hnz.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ahf.hnxiangtu.top

[R19] 数组长度
来源：http://uhz.zhoulong.xyz

echo "${#arr[@]}"
来源：http://yox.aizwys.cn

[R20] 关联数组（字典）
来源：http://sfb.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yfu.xuanzx.com

[R21] 字符串长度
来源：http://kqy.dashuyun.cn

echo "${#s}"
来源：http://kzl.zycfv.cn

[R22] 截取子串
来源：http://fno.pycfn.com

echo "${s:0:5}"
来源：http://haf.xylfe.cn

[R23] 字符串替换
来源：http://zug.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ypj.tanke756.top

[R24] 大小写转换
来源：http://lkl.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://pej.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://leq.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bif.haohaochexian.top

[R26] 命令替换
来源：http://lvk.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://hii.shzxlz.cn

[R27] 算术展开
来源：http://sou.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://zdp.zycfv.cn

[R28] 浮点运算
来源：http://gwj.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://bdh.xylfe.cn

[R29] 定义函数
来源：http://vor.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vkm.zhixingplan.top

[R30] 函数返回状态码
来源：http://qvz.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://bqf.hysaishi.cn

[R31] 局部变量
来源：http://hdh.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://vrz.gotoacloud.top

[R32] 参数个数校验
来源：http://qvr.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oaq.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://dif.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uyw.zhiwuduotai.top

[R34] 退出时清理
来源：http://mbf.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://avt.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://jzs.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vok.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://aom.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lgv.ehwqpu.com

[R37] 把输出赋给变量
来源：http://pxb.cheryme.top

files=$(ls -1)
来源：http://ehe.0kj1m.cn

[R38] 管道串联
来源：http://tkc.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://kuk.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://jar.vqdsnc.cn

cmd > out.log 2>&1
来源：http://fbk.zhijiandao.cn

[R40] 追加写日志
来源：http://hup.ehwqpu.com

echo "log" >> out.log
来源：http://mat.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ruy.yueranfly.top

cmd >/dev/null 2>&1
来源：http://mxw.chenjidiqi.icu

[R42] 输入重定向
来源：http://hnb.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://tne.dianchejie.cn

[R43] 按名字查找文件
来源：http://iel.jiagoushi.top

find . -name "*.log" -type f
来源：http://sak.shuidangran.top

[R44] 按修改时间查找
来源：http://bzz.sxryk.cn

find . -mtime -7 -type f
来源：http://hqi.chenzaomai.com

[R45] 批量删除
来源：http://bqr.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://nkf.wangdashe.top

[R46] 递归替换文件内容
来源：http://ngc.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yfk.haohaochexian.top

[R47] sed 单行替换
来源：http://uyi.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://plm.xuetiantiany.cn

[R48] awk 取指定列
来源：http://omv.fehbvm.com

awk '{print $1, $3}' a.txt
来源：http://bht.guowangkeji.top

[R49] awk 带条件
来源：http://tup.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mef.shangyingyoupin.top

[R50] awk 求和
来源：http://rzt.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://bxi.chenlongwang.top

[R51] 排序去重取前几
来源：http://sjn.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://afv.wangdashe.top

[R52] 统计行数
来源：http://ciu.chenlongwang.top

wc -l a.txt
来源：http://pvk.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://erc.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ixp.daria6918.cn

[R54] 比较两个文件
来源：http://fdt.guowangkeji.top

diff a.txt b.txt
来源：http://qvo.hfpthk.cn

[R55] 压缩与解压
来源：http://jmt.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mcm.zhongyouzk.top

[R56] 远程拷贝
来源：http://hoj.jyoumei.cn

scp file user@host:/path/
来源：http://sce.hesvh.cn

[R57] 远程执行命令
来源：http://gja.zhengqikj.top

ssh user@host 'uptime'
来源：http://sio.shanyushiyangtech.top

[R58] 下载文件
来源：http://upv.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sfu.haohaochexian.top

[R59] 发 POST JSON
来源：http://hwl.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://txz.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://bcl.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rwy.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://vef.kuanghao11.cn

df -h;  du -sh *
来源：http://beg.fehbvm.com

[R62] 找最占空间的文件
来源：http://uoc.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://pny.cashguo.top

[R63] 内存与进程
来源：http://aka.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://srd.fanxiaobao.xyz

[R64] 结束进程
来源：http://mjv.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://ztm.nanxuanxn.top

[R65] 查看端口占用
来源：http://gyc.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ulp.kuanghao11.cn

[R66] 定时任务
来源：http://fme.yuxming.cn

crontab -e;  crontab -l
来源：http://uxp.sweek.top

[R67] 生成随机十六进制串
来源：http://sil.svipenyu.cn


<!-- 参考信息 -->