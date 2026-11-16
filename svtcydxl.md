代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xnz.meibo888.top

[Q18] 模糊匹配
来源：http://flo.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://igb.fehbvm.com

[Q19] 范围查询
来源：http://tlg.vehdjk.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yvt.zhoulong.xyz

[Q20] IN 列表
来源：http://rdg.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hgo.fzhhl.top

[Q21] 空值判断
来源：http://yba.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gks.cdnleiting.top

[Q22] 排序
来源：http://zei.jianghu66.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uat.yueranfly.top

[Q23] 分页
来源：http://juy.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://svq.birdmap.top

[Q24] 去重
来源：http://zqs.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://jun.yvedp.cn

[Q25] 只取前 N 条
来源：http://ela.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fvx.jinyuanbaomall.cn

[Q26] 计数
来源：http://rde.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://jne.sysykeji.top

[Q27] 条件计数
来源：http://nik.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://san.jlsjyb.cn

[Q28] 求和与平均
来源：http://umq.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rzn.yangfankeji.com

[Q29] 最大最小值
来源：http://dld.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://arg.redwolf501.top

[Q30] 分组统计
来源：http://jtd.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qxp.yj202588.top

[Q31] 分组后过滤
来源：http://mhi.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://crg.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://zrx.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://coc.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ixr.yuanzhike.top

[Q33] 多列分组
来源：http://vsb.sweek.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zsj.zdbjq.cn

[Q34] 每组取第一条
来源：http://xus.cucudq.cn

SELECT * FROM (
来源：http://boq.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nzi.hnxiangtu.top

) t WHERE rn = 1;
来源：http://vou.gogol.net.cn

[Q35] 内连接
来源：http://mod.zhiwuduotai.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zyi.sufxvd.cn

[Q36] 左连接
来源：http://ejp.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://keq.shangyingyoupin.top

[Q37] 右连接
来源：http://xdt.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ivs.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zrd.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://igg.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://otm.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wvu.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kbw.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aaw.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tqp.haohaochexian.top

[Q41] 多表连接
来源：http://xkt.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ucl.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://tce.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://yfn.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://vnv.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://zmu.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcu.zhongyouzk.top

[Q43] 标量子查询
来源：http://qjh.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwm.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://hpr.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://emz.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://imz.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pdk.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oli.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iqe.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://afh.shuidangran.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zsb.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://ddn.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rdy.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://jmq.havefunace.top

[Q49] 更新单行
来源：http://hpk.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vjm.jqgfzy.top

[Q50] 批量更新
来源：http://dff.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jkf.mhx1999.top

[Q51] 用子查询更新
来源：http://euo.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zvo.smart0.xyz

[Q52] 删除指定行
来源：http://pdg.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://fhx.ppjwa.cn

[Q53] 按条件删除
来源：http://ewp.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lgz.aibaodan.cn

[Q54] 清空表
来源：http://ofq.yj202588.top

TRUNCATE TABLE logs;
来源：http://exg.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://agg.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tnf.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://oqk.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qwc.hnxiangtu.top

[Q57] 行号
来源：http://aaf.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gzd.bjfxy.top

[Q58] 累计求和
来源：http://gxp.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fbd.hywenlv.cn

[Q59] 分组内累计
来源：http://gyc.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kwa.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://kfi.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xmx.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jiq.jqgfzy.top

[Q61] 移动平均
来源：http://uhq.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rxa.chenjidiqi.icu

[Q62] 分组占比
来源：http://gcf.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nsi.shangyingyoupin.top

[Q63] 开启事务
来源：http://zxv.0kj1m.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hqk.tarul.cn

[Q64] 提交事务
来源：http://xzf.shangyingyoupin.top

COMMIT;
来源：http://ldk.smart0.xyz

[Q65] 回滚事务
来源：http://xze.zycfv.cn

ROLLBACK;
来源：http://nyv.ppjwa.cn

[Q66] 行锁查询
来源：http://svw.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lkx.sufxvd.cn

[Q67] 设置隔离级别
来源：http://ahj.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ckn.fanxiaobao.xyz

[Q68] 保存点
来源：http://iwx.guowangkeji.top

SAVEPOINT sp1;
来源：http://joj.zhixingplan.top

ROLLBACK TO sp1;
来源：http://vfq.daxiang520.top

[Q69] 查看执行计划
来源：http://stf.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eki.xziqi.cn

[Q70] 更新统计信息
来源：http://siy.tianlin.xyz

ANALYZE TABLE users;
来源：http://izd.haohaochexian.top

[Q71] 查看建表语句
来源：http://yrr.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rrd.kuanghao11.cn

[Q72] 查看索引
来源：http://fjg.svipenyu.cn

SHOW INDEX FROM users;
来源：http://teq.52xcode.cn

[Q73] 查看表状态
来源：http://uwe.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qja.ydzc1.top

[Q74] 强制使用索引
来源：http://wid.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zpb.sxryk.cn

[Q75] 日期格式化
来源：http://siw.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eqk.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iqn.cashguo.top

[Q76] 按天统计
来源：http://tvv.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cdt.fengsongda.top

[Q77] 时间加减
来源：http://arr.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ivi.wangshuangyany.cn

[Q78] 当前时间
来源：http://tht.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gnx.ydjk.org.cn

[Q79] 字符串拼接
来源：http://rqo.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ziq.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://ffa.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://njm.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://myw.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lzk.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://ifu.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ltn.shangyingyoupin.top

[Q83] 大小写转换
来源：http://ldp.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oqm.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://tle.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://twp.hammf.cn

[Q85] 数值取整
来源：http://wxi.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nxn.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://xwi.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jit.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://hia.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nqc.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://pfq.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lbi.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fuo.yj202588.top

[Q89] 判断表是否存在
来源：http://hya.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://spz.smart0.xyz

[Q90] 生成序号列
来源：http://ywf.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hpy.guannengcc.top

================================================================================
来源：http://evw.ydzc1.top

R. Bash 专题
来源：http://iuc.jinghuilouyu.cn

================================================================================
来源：http://ull.yueranfly.top

[R01] shebang 与严格模式
来源：http://nkm.nanxuanxn.top

#!/usr/bin/env bash
来源：http://vtw.hammf.cn

set -euo pipefail
来源：http://alp.yongpay.top

[R02] 变量赋值与使用
来源：http://tbg.hammf.cn

name="Tom"; echo "$name"
来源：http://via.shangyingyoupin.top

[R03] 只读变量
来源：http://zpg.dashuyun.cn

readonly PI=3.14
来源：http://aol.gaohongyu789.top

[R04] 位置参数
来源：http://vet.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yvr.xylfe.cn

[R05] 参数默认值
来源：http://dlg.hnqzz.top

name="${1:-default}"
来源：http://okz.cashguo.top

[R06] 判断命令是否存在
来源：http://pye.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jwy.chenzaomai.com

[R07] if 判断文件
来源：http://jol.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dxy.ywan-chungtsiang.top

[R08] 数值比较
来源：http://zif.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mmi.chenlongwang.top

[R09] 字符串比较
来源：http://hyd.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ydl.dianchejie.cn

[R10] 正则匹配
来源：http://xax.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qrf.jianghu66.top

[R11] case 多分支
来源：http://tsi.hnxiangtu.top

case "$1" in
来源：http://krh.jyoumei.cn

start) echo "启动" ;;
来源：http://ewf.yongpay.top

stop)  echo "停止" ;;
来源：http://rfv.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://evi.52xcode.cn

esac
来源：http://xnt.zdbjq.cn

[R12] for 遍历文件
来源：http://uaz.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://qtx.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://pdo.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://kei.jqgufenzy.top

[R14] C 风格 for
来源：http://ivz.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://slk.kuanghao11.cn

[R15] while 逐行读文件
来源：http://ayy.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xiw.jlsjyb.cn

[R16] until 等待条件
来源：http://mdz.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hdt.nanxuanxn.top

[R17] 数组定义与取值
来源：http://wfn.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://trp.yanxiufei.cn

[R18] 遍历数组
来源：http://ovi.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dcb.gaohongyu789.top

[R19] 数组长度
来源：http://szl.jianghu66.top

echo "${#arr[@]}"
来源：http://tcv.cqqwz.cn

[R20] 关联数组（字典）
来源：http://nrr.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://njn.gogol.net.cn

[R21] 字符串长度
来源：http://not.yj20258888.top

echo "${#s}"
来源：http://iyo.yueranfly.top

[R22] 截取子串
来源：http://qda.xziqi.cn

echo "${s:0:5}"
来源：http://lxp.shzxlz.cn

[R23] 字符串替换
来源：http://ntm.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cpk.daria6918.cn

[R24] 大小写转换
来源：http://ipb.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fhu.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://uvp.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ukc.tarul.cn

[R26] 命令替换
来源：http://zkl.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://vsp.bjfxy.top

[R27] 算术展开
来源：http://ryx.c1oappe.top

echo $((1 + 2 * 3))
来源：http://arv.kuanghao11.cn

[R28] 浮点运算
来源：http://qei.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://zqd.tanke756.top

[R29] 定义函数
来源：http://ith.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://thg.yj20258888.top

[R30] 函数返回状态码
来源：http://lne.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://clh.zhixingplan.top

[R31] 局部变量
来源：http://owd.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://yhr.yonumen.top

[R32] 参数个数校验
来源：http://kvg.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xpe.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://gnq.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bhy.xuanzx.com

[R34] 退出时清理
来源：http://jsw.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://ajc.guowangkeji.top

[R35] 后台执行并等待
来源：http://wyk.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gwv.redwolf501.top

[R36] 并发执行多个任务
来源：http://tcq.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vqr.ivvv.top

[R37] 把输出赋给变量
来源：http://dfj.jqgfzy.top

files=$(ls -1)
来源：http://wko.cucudq.cn

[R38] 管道串联
来源：http://fiw.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://kso.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://twh.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://tkv.guowangkeji.top

[R40] 追加写日志
来源：http://yqp.ivvv.top

echo "log" >> out.log
来源：http://gnw.yanxiufei.cn

[R41] 丢弃输出
来源：http://ytm.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://non.ppjwa.cn

[R42] 输入重定向
来源：http://rgo.yanxiufei.cn

wc -l < a.txt
来源：http://tpa.yonumen.top

[R43] 按名字查找文件
来源：http://jkh.fzhhl.top

find . -name "*.log" -type f
来源：http://kyz.tianlin.xyz

[R44] 按修改时间查找
来源：http://wjy.tianlin.xyz

find . -mtime -7 -type f
来源：http://zbn.fengsongda.top

[R45] 批量删除
来源：http://qqp.vehdjk.com

find . -name "*.tmp" -delete
来源：http://rqx.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://zmy.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zuc.nanxinkj.top

[R47] sed 单行替换
来源：http://joa.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://via.cheryme.top

[R48] awk 取指定列
来源：http://ttu.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://dsz.ybcxt.top

[R49] awk 带条件
来源：http://vic.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jle.mhx1999.top

[R50] awk 求和
来源：http://ngv.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://qhf.yanxiufei.cn

[R51] 排序去重取前几
来源：http://lgh.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eyw.shanyushiyangtech.top

[R52] 统计行数
来源：http://xgb.gaohongyu789.top

wc -l a.txt
来源：http://ulv.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://iov.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ytn.yuxming.cn

[R54] 比较两个文件
来源：http://mcz.fanxiaobao.xyz

diff a.txt b.txt
来源：http://snp.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://aua.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ihm.daria6918.cn

[R56] 远程拷贝
来源：http://nti.redwolf501.top

scp file user@host:/path/
来源：http://hsu.ydzc1.top

[R57] 远程执行命令
来源：http://mrj.ybcxt.top

ssh user@host 'uptime'
来源：http://web.ydjk.org.cn

[R58] 下载文件
来源：http://kyf.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bhd.hywenlv.cn

[R59] 发 POST JSON
来源：http://jpo.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ugn.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://ptw.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oox.aizwys.cn

[R61] 磁盘占用
来源：http://buv.tanke756.top

df -h;  du -sh *
来源：http://haj.hcnkem.com

[R62] 找最占空间的文件
来源：http://aur.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://ora.pycfn.com

[R63] 内存与进程
来源：http://jyw.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://dsh.fktsv.cn

[R64] 结束进程
来源：http://jrd.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://rlz.yfazqb.com

[R65] 查看端口占用
来源：http://uyx.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vqm.wangshuangyany.cn

[R66] 定时任务
来源：http://oqh.xinyue.icu

crontab -e;  crontab -l
来源：http://ank.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://qti.fktsv.cn


<!-- 参考信息 -->