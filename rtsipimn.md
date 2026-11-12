代发 wailian999

SELECT * FROM users;
来源：http://vli.zdqjudy.top

[Q16] 查询指定列
来源：http://nxg.guowangkeji.top

SELECT id, name FROM users;
来源：http://vcl.shanyushiyangtech.top

[Q17] 条件查询
来源：http://lkd.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zxf.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://kvi.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hmo.sufxvd.cn

[Q19] 范围查询
来源：http://yix.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ggv.jinqigufen.top

[Q20] IN 列表
来源：http://cto.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mba.c1oappe.top

[Q21] 空值判断
来源：http://njo.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pjp.cheryme.top

[Q22] 排序
来源：http://mak.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eqv.xingfuxueyuan.xyz

[Q23] 分页
来源：http://fpf.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mgc.fengsongda.top

[Q24] 去重
来源：http://yaj.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://ekw.daria6918.cn

[Q25] 只取前 N 条
来源：http://yrz.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://egd.shzxlz.cn

[Q26] 计数
来源：http://fxi.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://bpw.bbcook.cn

[Q27] 条件计数
来源：http://fdw.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ukk.shangyingyoupin.top

[Q28] 求和与平均
来源：http://taw.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ply.yueranfly.top

[Q29] 最大最小值
来源：http://mut.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymh.xinyue.icu

[Q30] 分组统计
来源：http://tlk.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fov.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://hxt.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://btp.ivvv.top

[Q32] 分组拼接字符串
来源：http://exw.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bkg.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jnn.jlsjyb.cn

[Q33] 多列分组
来源：http://cck.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kvs.fengsongda.top

[Q34] 每组取第一条
来源：http://ddz.bbcook.cn

SELECT * FROM (
来源：http://rfm.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oud.ybcxt.top

) t WHERE rn = 1;
来源：http://upu.hesvh.cn

[Q35] 内连接
来源：http://tpz.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hhg.hammf.cn

[Q36] 左连接
来源：http://xli.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uue.zhaomingkeji.xyz

[Q37] 右连接
来源：http://aga.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://klq.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://egl.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://erl.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://cmk.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pxi.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mhb.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tkc.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fko.fehbvm.com

[Q41] 多表连接
来源：http://ire.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://uqb.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://vki.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://iig.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://bjb.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://mgi.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mib.bbcook.cn

[Q43] 标量子查询
来源：http://osv.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pfh.kuanghao11.cn

[Q44] IN 子查询
来源：http://ptf.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://had.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://cvc.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iuf.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://yne.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dto.cheryme.top

[Q47] 与平均值比较
来源：http://zvx.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rua.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://jbs.bjfxy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fme.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://lah.cqqwz.cn

[Q49] 更新单行
来源：http://gnv.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fai.hfpthk.cn

[Q50] 批量更新
来源：http://bif.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nwn.jqgufenzy.top

[Q51] 用子查询更新
来源：http://xay.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://otz.tanke756.top

[Q52] 删除指定行
来源：http://ayh.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://gre.yanxiufei.cn

[Q53] 按条件删除
来源：http://nlf.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qzd.shuidangran.top

[Q54] 清空表
来源：http://msg.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://gek.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://gcw.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gbw.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://asp.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fmu.andypj.xyz

[Q57] 行号
来源：http://meg.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ljc.xuanzx.com

[Q58] 累计求和
来源：http://wky.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xxe.hammf.cn

[Q59] 分组内累计
来源：http://bnd.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iax.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://klo.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hmz.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rhz.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://ysa.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kzc.jinghuilouyu.cn

[Q62] 分组占比
来源：http://eeu.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ciw.c1oappe.top

[Q63] 开启事务
来源：http://nan.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dax.sxryk.cn

[Q64] 提交事务
来源：http://esx.fehbvm.com

COMMIT;
来源：http://lnk.dianchejie.cn

[Q65] 回滚事务
来源：http://uml.shanyushiyangkeji.top

ROLLBACK;
来源：http://cjs.aizwys.cn

[Q66] 行锁查询
来源：http://vwi.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mkk.fzhhl.top

[Q67] 设置隔离级别
来源：http://xtc.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hmb.bbcook.cn

[Q68] 保存点
来源：http://zpt.smart0.xyz

SAVEPOINT sp1;
来源：http://qdi.zdbjq.cn

ROLLBACK TO sp1;
来源：http://uac.ctjpmb.com

[Q69] 查看执行计划
来源：http://xnw.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bde.zhoulong.xyz

[Q70] 更新统计信息
来源：http://srs.yonumen.top

ANALYZE TABLE users;
来源：http://lgw.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://wgn.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wyy.vqdsnc.cn

[Q72] 查看索引
来源：http://zhv.fengsongda.top

SHOW INDEX FROM users;
来源：http://bmm.andypj.xyz

[Q73] 查看表状态
来源：http://ffx.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wop.yuanzhike.top

[Q74] 强制使用索引
来源：http://asy.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://roo.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://vcx.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xkc.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ele.sjlbkw.cn

[Q76] 按天统计
来源：http://qid.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fcw.hcnkem.com

[Q77] 时间加减
来源：http://tyg.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qhb.jqgfzy.top

[Q78] 当前时间
来源：http://tca.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cgq.aizwys.cn

[Q79] 字符串拼接
来源：http://zri.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://orx.bbcook.cn

[Q80] 字符串截取
来源：http://kww.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jyw.yvedp.cn

[Q81] 字符串替换
来源：http://ssy.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hpv.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://mhx.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jgo.zdqjudy.top

[Q83] 大小写转换
来源：http://vpa.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://oac.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://lqj.jinghuilouyu.cn

[Q85] 数值取整
来源：http://fdr.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vew.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://uxm.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qza.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://ith.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yrj.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://aqz.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zki.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sec.pycfn.com

[Q89] 判断表是否存在
来源：http://wis.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iqq.svipenyu.cn

[Q90] 生成序号列
来源：http://eze.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oor.316326.xyz

================================================================================
来源：http://mom.fktsv.cn

R. Bash 专题
来源：http://tar.yueranfly.top

================================================================================
来源：http://nzb.hnqzz.top

[R01] shebang 与严格模式
来源：http://oad.nwbrower.top

#!/usr/bin/env bash
来源：http://dns.guannengcc.top

set -euo pipefail
来源：http://bun.nwbrower.top

[R02] 变量赋值与使用
来源：http://xsj.shuidangran.top

name="Tom"; echo "$name"
来源：http://vxv.hesvh.cn

[R03] 只读变量
来源：http://uil.chenlongwang.top

readonly PI=3.14
来源：http://dhq.mhx1999.top

[R04] 位置参数
来源：http://rce.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jsx.sysykeji.top

[R05] 参数默认值
来源：http://zwb.sufxvd.cn

name="${1:-default}"
来源：http://fzb.smart0.xyz

[R06] 判断命令是否存在
来源：http://mmg.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nzc.hcnkem.com

[R07] if 判断文件
来源：http://ojd.chenzaomai.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ffq.zhiwuduotai.top

[R08] 数值比较
来源：http://yal.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://psq.hnxiangtu.top

[R09] 字符串比较
来源：http://nhk.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kzl.quarkkingdee.top

[R10] 正则匹配
来源：http://lky.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hmm.yanxiufei.cn

[R11] case 多分支
来源：http://lmb.xinyue.icu

case "$1" in
来源：http://woh.cashguo.top

start) echo "启动" ;;
来源：http://qzz.redwolf501.top

stop)  echo "停止" ;;
来源：http://lbu.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://jwr.dashuyun.cn

esac
来源：http://vhm.dianchejie.cn

[R12] for 遍历文件
来源：http://sea.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://gvr.fehbvm.com

[R13] for 计数循环
来源：http://xxf.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://nnp.cashguo.top

[R14] C 风格 for
来源：http://eaz.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tvz.52xcode.cn

[R15] while 逐行读文件
来源：http://zit.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://php.jyoumei.cn

[R16] until 等待条件
来源：http://wem.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sbz.bbcook.cn

[R17] 数组定义与取值
来源：http://czf.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://wic.tanke756.top

[R18] 遍历数组
来源：http://dii.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tvd.chenzaomai.com

[R19] 数组长度
来源：http://ldw.snrcjt.cn

echo "${#arr[@]}"
来源：http://liq.dashuyun.cn

[R20] 关联数组（字典）
来源：http://jgz.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://atu.chenzaomai.com

[R21] 字符串长度
来源：http://esh.zhijiandao.cn

echo "${#s}"
来源：http://top.aibaodan.cn

[R22] 截取子串
来源：http://dke.meibo888.top

echo "${s:0:5}"
来源：http://kpy.meibo888.top

[R23] 字符串替换
来源：http://plf.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://idf.xinyue.icu

[R24] 大小写转换
来源：http://qzh.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bcx.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://add.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://slp.shanyushiyangtech.top

[R26] 命令替换
来源：http://ixt.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://vek.havefunace.top

[R27] 算术展开
来源：http://hez.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://xab.ydzc1.top

[R28] 浮点运算
来源：http://asx.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://wyt.yangfankeji.com

[R29] 定义函数
来源：http://lzg.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://waf.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://woq.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://vgv.jiagoushi.top

[R31] 局部变量
来源：http://khn.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://noz.fzhhl.top

[R32] 参数个数校验
来源：http://hfd.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dkz.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://ntd.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rzx.yonumen.top

[R34] 退出时清理
来源：http://sfw.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vzc.daria6918.cn

[R35] 后台执行并等待
来源：http://zma.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ody.hesvh.cn

[R36] 并发执行多个任务
来源：http://zdc.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nup.hcnkem.com

[R37] 把输出赋给变量
来源：http://neb.iojbl.cn

files=$(ls -1)
来源：http://wdf.guannengcc.top

[R38] 管道串联
来源：http://wub.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://frp.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://kqf.hfpthk.cn

cmd > out.log 2>&1
来源：http://lhx.sweek.top

[R40] 追加写日志
来源：http://slh.xuanzx.com

echo "log" >> out.log
来源：http://aly.aizwys.cn

[R41] 丢弃输出
来源：http://vpu.andypj.xyz

cmd >/dev/null 2>&1
来源：http://oae.zhixingplan.top

[R42] 输入重定向
来源：http://flq.cdnleiting.top

wc -l < a.txt
来源：http://xwl.yongpay.top

[R43] 按名字查找文件
来源：http://yxw.pycfn.com

find . -name "*.log" -type f
来源：http://dzx.sweek.top

[R44] 按修改时间查找
来源：http://rym.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://cvx.ppjwa.cn

[R45] 批量删除
来源：http://wsv.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://jzd.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://rfg.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yzu.pycfn.com

[R47] sed 单行替换
来源：http://vzq.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://sej.mhx1999.top

[R48] awk 取指定列
来源：http://acn.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://cqb.bbcook.cn

[R49] awk 带条件
来源：http://ysc.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fzs.hysaishi.cn

[R50] awk 求和
来源：http://nct.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://jow.yj202588.top

[R51] 排序去重取前几
来源：http://req.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xgj.hnqzz.top

[R52] 统计行数
来源：http://rpu.hongshengwenyu.top

wc -l a.txt
来源：http://bon.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://fed.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dyh.gzhubu.top

[R54] 比较两个文件
来源：http://dut.sxryk.cn

diff a.txt b.txt
来源：http://nqk.hywenlv.cn

[R55] 压缩与解压
来源：http://kac.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nov.zhiwuduotai.top

[R56] 远程拷贝
来源：http://pvy.316326.xyz

scp file user@host:/path/
来源：http://idg.ivvv.top

[R57] 远程执行命令
来源：http://sff.birdmap.top

ssh user@host 'uptime'
来源：http://myo.yongpay.top

[R58] 下载文件
来源：http://qyb.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sdn.haohaochexian.top

[R59] 发 POST JSON
来源：http://uja.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ddc.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://qwk.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hic.pycfn.com

[R61] 磁盘占用
来源：http://obf.jyoumei.cn

df -h;  du -sh *
来源：http://cby.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://xjo.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://yaq.meibo888.top

[R63] 内存与进程
来源：http://zhr.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://vrv.xziqi.cn

[R64] 结束进程
来源：http://rqr.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://opo.bbcook.cn

[R65] 查看端口占用
来源：http://qfj.hammf.cn


<!-- 参考信息 -->