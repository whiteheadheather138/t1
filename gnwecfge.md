代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qbx.andypj.xyz

[Q18] 模糊匹配
来源：http://pva.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://myw.yuanzhike.top

[Q19] 范围查询
来源：http://rfr.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://reh.jinghuilouyu.cn

[Q20] IN 列表
来源：http://xgs.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uug.316326.xyz

[Q21] 空值判断
来源：http://gaz.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://asz.andypj.xyz

[Q22] 排序
来源：http://bbj.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jrp.cashguo.top

[Q23] 分页
来源：http://wlm.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://brj.yfazqb.com

[Q24] 去重
来源：http://grf.sweek.top

SELECT DISTINCT city FROM users;
来源：http://eub.chenlongwang.top

[Q25] 只取前 N 条
来源：http://zlf.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tna.shzxlz.cn

[Q26] 计数
来源：http://ffu.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://wsz.iojbl.cn

[Q27] 条件计数
来源：http://bvn.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tcm.jyoumei.cn

[Q28] 求和与平均
来源：http://cvc.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nmw.sweek.top

[Q29] 最大最小值
来源：http://snp.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bcf.fehbvm.com

[Q30] 分组统计
来源：http://uce.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fed.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://suu.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lef.hcnkem.com

[Q32] 分组拼接字符串
来源：http://rfr.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tnc.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltr.jinqigufen.top

[Q33] 多列分组
来源：http://yds.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cwe.zhijiandao.cn

[Q34] 每组取第一条
来源：http://wkl.316326.xyz

SELECT * FROM (
来源：http://jot.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ltv.hcnkem.com

) t WHERE rn = 1;
来源：http://udn.nanxinkj.top

[Q35] 内连接
来源：http://hoz.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hah.xinyue.icu

[Q36] 左连接
来源：http://fzb.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lfu.uphjek.com

[Q37] 右连接
来源：http://eld.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gcc.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://mug.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://arj.aizwys.cn

[Q39] 自连接（查上下级）
来源：http://xfd.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://wan.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uaq.zhiwuduotai.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ugd.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qoh.sweek.top

[Q41] 多表连接
来源：http://ntb.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wwk.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://mhs.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://vuv.cashguo.top

[Q42] 连接条件附加过滤
来源：http://vco.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://fvd.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tbh.ydjk.org.cn

[Q43] 标量子查询
来源：http://ryi.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iwt.zdbjq.cn

[Q44] IN 子查询
来源：http://acw.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rpr.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://mqh.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oqq.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://pbj.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://obd.yj20258888.top

[Q47] 与平均值比较
来源：http://cnf.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://szh.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://tam.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dqd.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://vsi.ydjk.org.cn

[Q49] 更新单行
来源：http://tcs.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yku.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://csc.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wue.cucudq.cn

[Q51] 用子查询更新
来源：http://uxe.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ucx.cqqwz.cn

[Q52] 删除指定行
来源：http://ure.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://atd.sufxvd.cn

[Q53] 按条件删除
来源：http://qjn.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bnz.bjfxy.top

[Q54] 清空表
来源：http://eho.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://nhn.daria6918.cn

[Q55] 排名（并列占位）
来源：http://osa.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uys.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://ldy.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xks.epnwcf.com

[Q57] 行号
来源：http://nfb.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ydt.yongpay.top

[Q58] 累计求和
来源：http://xkq.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aaq.nwbrower.top

[Q59] 分组内累计
来源：http://qbg.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lgp.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://wwl.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gkq.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xqt.jqgfzy.top

[Q61] 移动平均
来源：http://dgz.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bzg.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://fdo.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://erk.hysaishi.cn

[Q63] 开启事务
来源：http://xxd.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fxu.ctjpmb.com

[Q64] 提交事务
来源：http://flr.zhiwuduotai.top

COMMIT;
来源：http://dlz.bjfxy.top

[Q65] 回滚事务
来源：http://glp.52xcode.cn

ROLLBACK;
来源：http://xcx.zdqjudy.top

[Q66] 行锁查询
来源：http://brz.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dbq.mhx1999.top

[Q67] 设置隔离级别
来源：http://ccc.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xfo.316326.xyz

[Q68] 保存点
来源：http://biz.cucudq.cn

SAVEPOINT sp1;
来源：http://rrj.cashguo.top

ROLLBACK TO sp1;
来源：http://sku.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://tky.bbcook.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yky.gogol.net.cn

[Q70] 更新统计信息
来源：http://iot.tarul.cn

ANALYZE TABLE users;
来源：http://oxs.mhx1999.top

[Q71] 查看建表语句
来源：http://vbp.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mar.fktsv.cn

[Q72] 查看索引
来源：http://evs.fehbvm.com

SHOW INDEX FROM users;
来源：http://gqi.xylfe.cn

[Q73] 查看表状态
来源：http://kzm.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pst.yonumen.top

[Q74] 强制使用索引
来源：http://lqg.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rki.iojbl.cn

[Q75] 日期格式化
来源：http://ptn.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jdn.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vfp.cheryme.top

[Q76] 按天统计
来源：http://pli.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pzw.hfpthk.cn

[Q77] 时间加减
来源：http://zwe.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lye.redwolf501.top

[Q78] 当前时间
来源：http://bai.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dor.tian-w.cn

[Q79] 字符串拼接
来源：http://sgf.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://axy.wangshuangyany.cn

[Q80] 字符串截取
来源：http://xbd.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yfb.svipenyu.cn

[Q81] 字符串替换
来源：http://xtr.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cya.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://asy.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://laf.kuanghao11.cn

[Q83] 大小写转换
来源：http://gzs.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://grq.fktsv.cn

[Q84] 去除首尾空格
来源：http://niy.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://djf.yj20258888.top

[Q85] 数值取整
来源：http://lkc.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iqv.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://xxc.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tid.xuanzx.com

[Q87] JSON 字段做条件
来源：http://gyp.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fev.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://lvc.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jgy.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vqc.ydzc1.top

[Q89] 判断表是否存在
来源：http://nvq.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://inh.wangshuangyany.cn

[Q90] 生成序号列
来源：http://gcd.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xng.wangdashe.top

================================================================================
来源：http://zen.jinqigfzy.top

R. Bash 专题
来源：http://lxr.tarul.cn

================================================================================
来源：http://oem.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://ame.hysaishi.cn

#!/usr/bin/env bash
来源：http://nyq.yvedp.cn

set -euo pipefail
来源：http://jej.jqgfzy.top

[R02] 变量赋值与使用
来源：http://nlr.gogol.net.cn

name="Tom"; echo "$name"
来源：http://bys.quarkkingdee.top

[R03] 只读变量
来源：http://yzu.tarul.cn

readonly PI=3.14
来源：http://cyh.yj20258.top

[R04] 位置参数
来源：http://prl.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ktr.ehwqpu.com

[R05] 参数默认值
来源：http://piv.sxryk.cn

name="${1:-default}"
来源：http://syh.hnqzz.top

[R06] 判断命令是否存在
来源：http://het.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dim.zhijiandao.cn

[R07] if 判断文件
来源：http://jlo.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dst.hcnkem.com

[R08] 数值比较
来源：http://iqn.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hka.cheryme.top

[R09] 字符串比较
来源：http://xlu.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qjn.jinghuilouyu.cn

[R10] 正则匹配
来源：http://lmq.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vzw.zhengqikj.top

[R11] case 多分支
来源：http://sfc.pycfn.com

case "$1" in
来源：http://lfc.gzhubu.top

start) echo "启动" ;;
来源：http://fol.cucudq.cn

stop)  echo "停止" ;;
来源：http://oac.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://wxu.sysykeji.top

esac
来源：http://rok.jinqigfzy.top

[R12] for 遍历文件
来源：http://dkd.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://gna.shuidangran.top

[R13] for 计数循环
来源：http://ldp.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://isv.yvedp.cn

[R14] C 风格 for
来源：http://gcr.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://unp.zhongyouzk.top

[R15] while 逐行读文件
来源：http://gdy.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kao.shuidangran.top

[R16] until 等待条件
来源：http://eck.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zba.meibo888.top

[R17] 数组定义与取值
来源：http://yzm.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://htm.snrcjt.cn

[R18] 遍历数组
来源：http://ulw.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://npm.fktsv.cn

[R19] 数组长度
来源：http://cdr.hfpthk.cn

echo "${#arr[@]}"
来源：http://npy.yueranfly.top

[R20] 关联数组（字典）
来源：http://asq.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://suy.ydjk.org.cn

[R21] 字符串长度
来源：http://isy.tianlin.xyz

echo "${#s}"
来源：http://tkb.kuanghao11.cn

[R22] 截取子串
来源：http://zzz.pycfn.com

echo "${s:0:5}"
来源：http://fjh.yanxiufei.cn

[R23] 字符串替换
来源：http://flb.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kzd.cdnleiting.top

[R24] 大小写转换
来源：http://smu.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://phh.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://lpj.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sww.shangyingyoupin.top

[R26] 命令替换
来源：http://efc.tarul.cn

now=$(date +%F); echo "$now"
来源：http://vqn.wangdashe.top

[R27] 算术展开
来源：http://bbf.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://gpt.yj202588.top

[R28] 浮点运算
来源：http://eii.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://rul.yanxiufei.cn

[R29] 定义函数
来源：http://vqq.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gtw.sweek.top

[R30] 函数返回状态码
来源：http://vtk.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://luu.ydjk.org.cn

[R31] 局部变量
来源：http://dtt.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://njw.316326.xyz

[R32] 参数个数校验
来源：http://ple.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lsz.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://vaz.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cov.svipenyu.cn

[R34] 退出时清理
来源：http://rtc.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://vbw.zhijiandao.cn

[R35] 后台执行并等待
来源：http://ufk.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qqu.svipenyu.cn

[R36] 并发执行多个任务
来源：http://pnk.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zhq.vehdjk.com

[R37] 把输出赋给变量
来源：http://mjb.zhaomingkeji.xyz

files=$(ls -1)
来源：http://csr.xziqi.cn

[R38] 管道串联
来源：http://itk.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://woc.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://nld.kuanghao11.cn

cmd > out.log 2>&1
来源：http://rks.chenjidiqi.icu

[R40] 追加写日志
来源：http://pnb.shanyushiyangtech.top

echo "log" >> out.log
来源：http://alb.zycfv.cn

[R41] 丢弃输出
来源：http://gar.bbcook.cn

cmd >/dev/null 2>&1
来源：http://zps.zhijiandao.cn

[R42] 输入重定向
来源：http://nrg.epnwcf.com

wc -l < a.txt
来源：http://mvv.zhoulong.xyz

[R43] 按名字查找文件
来源：http://yit.cqqwz.cn

find . -name "*.log" -type f
来源：http://dcq.guowangkeji.top

[R44] 按修改时间查找
来源：http://arc.yanxiufei.cn

find . -mtime -7 -type f
来源：http://ixa.cqqwz.cn

[R45] 批量删除
来源：http://pfx.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://icm.vehdjk.com

[R46] 递归替换文件内容
来源：http://llw.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jkz.yongpay.top

[R47] sed 单行替换
来源：http://fla.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://tsj.uphjek.com

[R48] awk 取指定列
来源：http://jib.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://vmj.fanxiaobao.xyz

[R49] awk 带条件
来源：http://yqs.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cqn.wangdashe.top

[R50] awk 求和
来源：http://yrd.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bke.cqqwz.cn

[R51] 排序去重取前几
来源：http://xbj.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bpg.aibaodan.cn

[R52] 统计行数
来源：http://xwe.dianchejie.cn

wc -l a.txt
来源：http://tzc.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://iru.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pmk.sweek.top

[R54] 比较两个文件
来源：http://nqe.bjfxy.top

diff a.txt b.txt
来源：http://fby.yj202588.top

[R55] 压缩与解压
来源：http://kix.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gkn.gogol.net.cn

[R56] 远程拷贝
来源：http://fsq.shangyingyoupin.top

scp file user@host:/path/
来源：http://uxv.ivvv.top

[R57] 远程执行命令
来源：http://uis.wangdashe.top

ssh user@host 'uptime'
来源：http://cio.hongshengwenyu.top

[R58] 下载文件
来源：http://vob.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pwc.ydjk.org.cn

[R59] 发 POST JSON
来源：http://nik.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qsl.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://lrm.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hhh.tanke756.top

[R61] 磁盘占用
来源：http://bxs.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://eyn.sufxvd.cn

[R62] 找最占空间的文件
来源：http://eip.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://ozq.quarkkingdee.top

[R63] 内存与进程
来源：http://zzq.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://nfu.yfazqb.com

[R64] 结束进程
来源：http://sop.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://jca.yanxiufei.cn

[R65] 查看端口占用
来源：http://joy.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ymp.gaohongyu789.top

[R66] 定时任务
来源：http://gvr.meibo888.top

crontab -e;  crontab -l
来源：http://bcq.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://xhg.sufxvd.cn


<!-- 参考信息 -->