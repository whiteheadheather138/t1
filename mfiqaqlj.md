代发 wailian999

SELECT * FROM users;
来源：http://bst.yangfankeji.com

[Q16] 查询指定列
来源：http://smk.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://gsc.ctjpmb.com

[Q17] 条件查询
来源：http://sam.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yqm.yangfankeji.com

[Q18] 模糊匹配
来源：http://wto.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ytb.meibo888.top

[Q19] 范围查询
来源：http://uru.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dwn.shzxlz.cn

[Q20] IN 列表
来源：http://tca.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zvs.hongshengwenyu.top

[Q21] 空值判断
来源：http://npe.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cmo.zdqjudy.top

[Q22] 排序
来源：http://qjo.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://thz.ivvv.top

[Q23] 分页
来源：http://llb.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jsi.hongshengwenyu.top

[Q24] 去重
来源：http://jvs.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://vjs.guannengcc.top

[Q25] 只取前 N 条
来源：http://gpi.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fxf.dashuyun.cn

[Q26] 计数
来源：http://rct.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://lsf.tian-w.cn

[Q27] 条件计数
来源：http://afv.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qwt.aibaodan.cn

[Q28] 求和与平均
来源：http://pfq.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lij.yonumen.top

[Q29] 最大最小值
来源：http://skq.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sdp.gzhubu.top

[Q30] 分组统计
来源：http://pxr.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uiq.cucudq.cn

[Q31] 分组后过滤
来源：http://vba.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vty.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://pbr.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nob.snrcjt.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bdg.snrcjt.cn

[Q33] 多列分组
来源：http://yav.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oil.zycfv.cn

[Q34] 每组取第一条
来源：http://fka.ydjk.org.cn

SELECT * FROM (
来源：http://uub.bjfxy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bya.cheryme.top

) t WHERE rn = 1;
来源：http://krb.hcnkem.com

[Q35] 内连接
来源：http://igw.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hbr.smart0.xyz

[Q36] 左连接
来源：http://aaw.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eee.fzhhl.top

[Q37] 右连接
来源：http://iyp.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ifk.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://yrb.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yqn.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://wem.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bou.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ldq.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zew.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://urq.andypj.xyz

[Q41] 多表连接
来源：http://srh.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ndn.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://vem.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://ber.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://lfa.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://loe.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hkv.ybcxt.top

[Q43] 标量子查询
来源：http://dqm.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lvm.tian-w.cn

[Q44] IN 子查询
来源：http://dfz.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rmq.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://nxt.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ikt.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://ljl.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://irt.yanxiufei.cn

[Q47] 与平均值比较
来源：http://txs.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wzz.birdmap.top

[Q48] CTE 公用表表达式
来源：http://yaf.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xxt.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://jvu.yuxming.cn

[Q49] 更新单行
来源：http://khi.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vzf.chenjidiqi.icu

[Q50] 批量更新
来源：http://yzf.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jww.sxryk.cn

[Q51] 用子查询更新
来源：http://leh.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bvs.zycfv.cn

[Q52] 删除指定行
来源：http://zqe.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://cyh.yvedp.cn

[Q53] 按条件删除
来源：http://ovd.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dzu.shangyingyoupin.top

[Q54] 清空表
来源：http://vus.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://zdx.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://lkf.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fzq.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://ksr.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rnj.fzhhl.top

[Q57] 行号
来源：http://ojr.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://omv.yvedp.cn

[Q58] 累计求和
来源：http://lpn.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ruq.cdnleiting.top

[Q59] 分组内累计
来源：http://bix.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eum.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://ryd.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bzr.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpq.meibo888.top

[Q61] 移动平均
来源：http://pqu.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mak.sxryk.cn

[Q62] 分组占比
来源：http://avz.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ikz.quarkkingdee.top

[Q63] 开启事务
来源：http://kww.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wbc.meibo888.top

[Q64] 提交事务
来源：http://our.xinyue.icu

COMMIT;
来源：http://ejv.shuidangran.top

[Q65] 回滚事务
来源：http://qbr.redwolf501.top

ROLLBACK;
来源：http://fov.shangyingyoupin.top

[Q66] 行锁查询
来源：http://uai.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ybo.52xcode.cn

[Q67] 设置隔离级别
来源：http://jay.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pir.ydzc1.top

[Q68] 保存点
来源：http://qei.andypj.xyz

SAVEPOINT sp1;
来源：http://enh.ivvv.top

ROLLBACK TO sp1;
来源：http://edi.c1oappe.top

[Q69] 查看执行计划
来源：http://khs.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vyv.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://tav.aibaodan.cn

ANALYZE TABLE users;
来源：http://yvr.yvedp.cn

[Q71] 查看建表语句
来源：http://cli.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fqo.xinyue.icu

[Q72] 查看索引
来源：http://czt.ivvv.top

SHOW INDEX FROM users;
来源：http://fpo.sysykeji.top

[Q73] 查看表状态
来源：http://lmv.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bqf.zhijiandao.cn

[Q74] 强制使用索引
来源：http://vge.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xmo.yj202588.top

[Q75] 日期格式化
来源：http://oow.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blw.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pqj.jlsjyb.cn

[Q76] 按天统计
来源：http://met.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zkg.tarul.cn

[Q77] 时间加减
来源：http://gjd.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qmh.gaohongyu789.top

[Q78] 当前时间
来源：http://uot.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://akl.0kj1m.cn

[Q79] 字符串拼接
来源：http://kvq.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://saa.sxryk.cn

[Q80] 字符串截取
来源：http://vgz.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uaf.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://ahe.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kyd.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://cqy.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xdj.yanxiufei.cn

[Q83] 大小写转换
来源：http://myb.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://odk.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://ksn.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://xfn.sufxvd.cn

[Q85] 数值取整
来源：http://nmm.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://olv.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://xux.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tnj.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://fvp.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qaw.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://zxn.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zzh.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bld.zdbjq.cn

[Q89] 判断表是否存在
来源：http://gaq.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nuw.nwbrower.top

[Q90] 生成序号列
来源：http://ony.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zuv.yj20258.top

================================================================================
来源：http://jpt.havefunace.top

R. Bash 专题
来源：http://tlo.cashguo.top

================================================================================
来源：http://jbk.aizwys.cn

[R01] shebang 与严格模式
来源：http://tgz.jianghu66.top

#!/usr/bin/env bash
来源：http://kbk.zhengqikj.top

set -euo pipefail
来源：http://pha.hysaishi.cn

[R02] 变量赋值与使用
来源：http://ayw.andypj.xyz

name="Tom"; echo "$name"
来源：http://dfy.yueranfly.top

[R03] 只读变量
来源：http://jjo.jianghu66.top

readonly PI=3.14
来源：http://isd.ppjwa.cn

[R04] 位置参数
来源：http://dgb.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qbd.epnwcf.com

[R05] 参数默认值
来源：http://fmd.zhijiandao.cn

name="${1:-default}"
来源：http://vrs.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://flp.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wmy.yfazqb.com

[R07] if 判断文件
来源：http://ixz.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eve.fanxiaobao.xyz

[R08] 数值比较
来源：http://cse.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zpg.zdqjudy.top

[R09] 字符串比较
来源：http://mts.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bbt.zhengqikj.top

[R10] 正则匹配
来源：http://pai.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://okv.sxryk.cn

[R11] case 多分支
来源：http://bvd.smart0.xyz

case "$1" in
来源：http://rkg.epnwcf.com

start) echo "启动" ;;
来源：http://xlk.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://hvk.vehdjk.com

*)     echo "未知命令" ;;
来源：http://goc.feifeiyinyue.top

esac
来源：http://bdk.kuanghao11.cn

[R12] for 遍历文件
来源：http://kzz.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://tgc.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://fxb.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://zhx.haohaochexian.top

[R14] C 风格 for
来源：http://jgy.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jsd.cucudq.cn

[R15] while 逐行读文件
来源：http://vik.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kjk.chenzaomai.com

[R16] until 等待条件
来源：http://bfm.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zwn.chenlongwang.top

[R17] 数组定义与取值
来源：http://tul.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://roj.shzxlz.cn

[R18] 遍历数组
来源：http://tuk.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fkr.jinqigufen.top

[R19] 数组长度
来源：http://wwg.hywenlv.cn

echo "${#arr[@]}"
来源：http://sil.52xcode.cn

[R20] 关联数组（字典）
来源：http://xcr.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cbp.yvedp.cn

[R21] 字符串长度
来源：http://adv.andypj.xyz

echo "${#s}"
来源：http://zji.zhijiandao.cn

[R22] 截取子串
来源：http://eby.vqdsnc.cn

echo "${s:0:5}"
来源：http://qii.fanxiaobao.xyz

[R23] 字符串替换
来源：http://mld.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ysk.zdqjudy.top

[R24] 大小写转换
来源：http://pwf.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zhg.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://vro.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pji.zhiwuduotai.top

[R26] 命令替换
来源：http://dsy.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://bbz.9152youxi.cn

[R27] 算术展开
来源：http://oov.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://jjf.hnqzz.top

[R28] 浮点运算
来源：http://uoy.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://mdo.jyoumei.cn

[R29] 定义函数
来源：http://jug.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ikw.9152youxi.cn

[R30] 函数返回状态码
来源：http://zzh.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://aym.yuanzhike.top

[R31] 局部变量
来源：http://lts.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://sbu.redwolf501.top

[R32] 参数个数校验
来源：http://zao.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://udv.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://lmr.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hyr.yj20258.top

[R34] 退出时清理
来源：http://upk.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ubs.c1oappe.top

[R35] 后台执行并等待
来源：http://njr.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lof.yueranfly.top

[R36] 并发执行多个任务
来源：http://dkc.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://chl.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://smy.yongpay.top

files=$(ls -1)
来源：http://ohq.wangdashe.top

[R38] 管道串联
来源：http://oix.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://lnj.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://cpp.snrcjt.cn

cmd > out.log 2>&1
来源：http://hmt.shzxlz.cn

[R40] 追加写日志
来源：http://cly.hnqzz.top

echo "log" >> out.log
来源：http://nhy.iojbl.cn

[R41] 丢弃输出
来源：http://nui.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://nvr.tarul.cn

[R42] 输入重定向
来源：http://wdz.xziqi.cn

wc -l < a.txt
来源：http://ytu.tanke756.top

[R43] 按名字查找文件
来源：http://qki.xylfe.cn

find . -name "*.log" -type f
来源：http://yzn.ybcxt.top

[R44] 按修改时间查找
来源：http://uyw.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://lok.guannengcc.top

[R45] 批量删除
来源：http://bve.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://skh.jiagoushi.top

[R46] 递归替换文件内容
来源：http://xbq.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cjj.chenjidiqi.icu

[R47] sed 单行替换
来源：http://zcg.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cql.shuidangran.top

[R48] awk 取指定列
来源：http://xyw.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://cbn.xuanzx.com

[R49] awk 带条件
来源：http://ukl.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nrf.aibaodan.cn

[R50] awk 求和
来源：http://sap.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dah.gotoacloud.top

[R51] 排序去重取前几
来源：http://vzt.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cjc.svipenyu.cn

[R52] 统计行数
来源：http://slj.redwolf501.top

wc -l a.txt
来源：http://qdt.sweek.top

[R53] 查看文件头与实时尾
来源：http://kwd.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mcf.zhijiandao.cn

[R54] 比较两个文件
来源：http://klk.redwolf501.top

diff a.txt b.txt
来源：http://hdz.fengsongda.top

[R55] 压缩与解压
来源：http://uon.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vzt.redwolf501.top

[R56] 远程拷贝
来源：http://kao.dianchejie.cn

scp file user@host:/path/
来源：http://mng.smart0.xyz

[R57] 远程执行命令
来源：http://njq.ydjk.org.cn

ssh user@host 'uptime'
来源：http://ssq.cashguo.top

[R58] 下载文件
来源：http://wlw.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://msc.ctjpmb.com

[R59] 发 POST JSON
来源：http://xja.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bgo.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://jxh.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qnp.guannengcc.top

[R61] 磁盘占用
来源：http://ehd.pycfn.com

df -h;  du -sh *
来源：http://bqa.uphjek.com

[R62] 找最占空间的文件
来源：http://thb.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://rzq.cashguo.top

[R63] 内存与进程
来源：http://mfh.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://rfe.jiagoushi.top

[R64] 结束进程
来源：http://zgv.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://ojk.xinyue.icu

[R65] 查看端口占用
来源：http://pqv.yj20258888.top


<!-- 参考信息 -->