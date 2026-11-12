代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://lhc.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jvc.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://axv.yvedp.cn

[Q15] 查询全部
来源：http://xie.cdnleiting.top

SELECT * FROM users;
来源：http://efc.fehbvm.com

[Q16] 查询指定列
来源：http://viq.aizwys.cn

SELECT id, name FROM users;
来源：http://ysr.yangfankeji.com

[Q17] 条件查询
来源：http://hjk.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ovg.gotoacloud.top

[Q18] 模糊匹配
来源：http://mxh.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://umk.yj20258.top

[Q19] 范围查询
来源：http://jat.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://woy.daria6918.cn

[Q20] IN 列表
来源：http://lef.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rav.birdmap.top

[Q21] 空值判断
来源：http://lqz.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wyf.ehwqpu.com

[Q22] 排序
来源：http://ovm.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jqa.xziqi.cn

[Q23] 分页
来源：http://qtk.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wxa.smart0.xyz

[Q24] 去重
来源：http://dgw.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://wkm.nanxinkj.top

[Q25] 只取前 N 条
来源：http://lzq.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://flt.yongpay.top

[Q26] 计数
来源：http://wnq.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://sjp.jinqigfzy.top

[Q27] 条件计数
来源：http://uph.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qxy.gogol.net.cn

[Q28] 求和与平均
来源：http://cyt.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qfn.tianlin.xyz

[Q29] 最大最小值
来源：http://vda.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yix.epnwcf.com

[Q30] 分组统计
来源：http://jhv.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fng.vqdsnc.cn

[Q31] 分组后过滤
来源：http://uzs.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://orv.redwolf501.top

[Q32] 分组拼接字符串
来源：http://eyo.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nit.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://weh.birdmap.top

[Q33] 多列分组
来源：http://wth.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://inn.hywenlv.cn

[Q34] 每组取第一条
来源：http://ggd.sysykeji.top

SELECT * FROM (
来源：http://han.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hbm.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://mcm.guowangkeji.top

[Q35] 内连接
来源：http://whn.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mdd.shangyingyoupin.top

[Q36] 左连接
来源：http://bko.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://typ.hywenlv.cn

[Q37] 右连接
来源：http://nxg.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kwv.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://gja.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rrr.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://myj.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qaz.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lrk.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bvn.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bsv.dashuyun.cn

[Q41] 多表连接
来源：http://vvi.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://azt.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://wfx.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://zpf.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://xdd.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://xgk.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://egh.ydjk.org.cn

[Q43] 标量子查询
来源：http://cox.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fkc.wangshuangyany.cn

[Q44] IN 子查询
来源：http://gld.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rmm.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://ruf.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ccq.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://ptt.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://biw.smart0.xyz

[Q47] 与平均值比较
来源：http://fmw.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ywk.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://crr.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oip.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://iao.ydjk.org.cn

[Q49] 更新单行
来源：http://hte.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xgu.52xcode.cn

[Q50] 批量更新
来源：http://dxu.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kfj.gaohongyu789.top

[Q51] 用子查询更新
来源：http://cjj.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bgh.smart0.xyz

[Q52] 删除指定行
来源：http://urm.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://qvx.pycfn.com

[Q53] 按条件删除
来源：http://fbg.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ezi.yonumen.top

[Q54] 清空表
来源：http://eam.gzhubu.top

TRUNCATE TABLE logs;
来源：http://qzz.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://nef.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hdp.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://rco.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vgk.fehbvm.com

[Q57] 行号
来源：http://fqg.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dcw.cucudq.cn

[Q58] 累计求和
来源：http://nmd.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qzo.hnqzz.top

[Q59] 分组内累计
来源：http://yss.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vfv.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://bgg.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zzp.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jko.gaohongyu789.top

[Q61] 移动平均
来源：http://ikp.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cjx.bbcook.cn

[Q62] 分组占比
来源：http://loy.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nlm.ivvv.top

[Q63] 开启事务
来源：http://yyd.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://swu.smart0.xyz

[Q64] 提交事务
来源：http://mpp.zdbjq.cn

COMMIT;
来源：http://pyg.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://iap.yvedp.cn

ROLLBACK;
来源：http://gyc.zhijiandao.cn

[Q66] 行锁查询
来源：http://ppz.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xwn.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://eru.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zzl.ywan-chungtsiang.top

[Q68] 保存点
来源：http://rvn.hywenlv.cn

SAVEPOINT sp1;
来源：http://hjl.0kj1m.cn

ROLLBACK TO sp1;
来源：http://xqu.xinyue.icu

[Q69] 查看执行计划
来源：http://nof.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://czr.tanke756.top

[Q70] 更新统计信息
来源：http://gnx.cqqwz.cn

ANALYZE TABLE users;
来源：http://uap.vehdjk.com

[Q71] 查看建表语句
来源：http://ubn.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oqt.aibaodan.cn

[Q72] 查看索引
来源：http://dlb.hesvh.cn

SHOW INDEX FROM users;
来源：http://jqx.tian-w.cn

[Q73] 查看表状态
来源：http://bvz.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://inl.9152youxi.cn

[Q74] 强制使用索引
来源：http://tpe.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vmn.andypj.xyz

[Q75] 日期格式化
来源：http://wuc.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bsp.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://npw.zhiwuduotai.top

[Q76] 按天统计
来源：http://aey.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yzn.yj20258888.top

[Q77] 时间加减
来源：http://gul.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kxg.sysykeji.top

[Q78] 当前时间
来源：http://qsd.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gcw.zhongyouzk.top

[Q79] 字符串拼接
来源：http://bkg.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wzk.dashuyun.cn

[Q80] 字符串截取
来源：http://big.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xjz.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://jzi.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qbf.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://zxk.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://npr.chenlongwang.top

[Q83] 大小写转换
来源：http://vue.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oaw.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://bpx.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://efs.sxryk.cn

[Q85] 数值取整
来源：http://vpj.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hna.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://xgt.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hci.aizwys.cn

[Q87] JSON 字段做条件
来源：http://agk.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fxc.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://nmc.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://koi.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lkv.dianchejie.cn

[Q89] 判断表是否存在
来源：http://zbf.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rfu.iojbl.cn

[Q90] 生成序号列
来源：http://war.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qme.redwolf501.top

================================================================================
来源：http://ilx.smart0.xyz

R. Bash 专题
来源：http://hao.bbcook.cn

================================================================================
来源：http://gkg.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://rdo.ybcxt.top

#!/usr/bin/env bash
来源：http://ufo.tian-w.cn

set -euo pipefail
来源：http://dmx.yonumen.top

[R02] 变量赋值与使用
来源：http://klk.smart0.xyz

name="Tom"; echo "$name"
来源：http://kil.pycfn.com

[R03] 只读变量
来源：http://mko.fengsongda.top

readonly PI=3.14
来源：http://rxb.pengpengdd.cyou

[R04] 位置参数
来源：http://ins.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ayc.gaohongyu789.top

[R05] 参数默认值
来源：http://rts.andypj.xyz

name="${1:-default}"
来源：http://upo.hcnkem.com

[R06] 判断命令是否存在
来源：http://dyc.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wyi.tianlin.xyz

[R07] if 判断文件
来源：http://ziw.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xnv.epnwcf.com

[R08] 数值比较
来源：http://meg.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pxa.bjfxy.top

[R09] 字符串比较
来源：http://wbo.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hna.vqdsnc.cn

[R10] 正则匹配
来源：http://sxc.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://koo.jqgufenzy.top

[R11] case 多分支
来源：http://yld.shzxlz.cn

case "$1" in
来源：http://tub.jqgufenzy.top

start) echo "启动" ;;
来源：http://tdf.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://rqq.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://sse.ydjk.org.cn

esac
来源：http://snv.tianlin.xyz

[R12] for 遍历文件
来源：http://cvc.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://eoj.0kj1m.cn

[R13] for 计数循环
来源：http://zsz.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://vgl.zycfv.cn

[R14] C 风格 for
来源：http://plf.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jbl.shuidangran.top

[R15] while 逐行读文件
来源：http://ajf.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://usk.tianlin.xyz

[R16] until 等待条件
来源：http://xww.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zcj.havefunace.top

[R17] 数组定义与取值
来源：http://vys.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://pqd.hnxiangtu.top

[R18] 遍历数组
来源：http://mml.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://psj.sweek.top

[R19] 数组长度
来源：http://pzv.jinqigfzy.top

echo "${#arr[@]}"
来源：http://jxs.shzxlz.cn

[R20] 关联数组（字典）
来源：http://trc.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uyl.316326.xyz

[R21] 字符串长度
来源：http://lby.ppjwa.cn

echo "${#s}"
来源：http://ikt.zhongyouzk.top

[R22] 截取子串
来源：http://dya.vqdsnc.cn

echo "${s:0:5}"
来源：http://tfn.yfazqb.com

[R23] 字符串替换
来源：http://uhz.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nzx.birdmap.top

[R24] 大小写转换
来源：http://iiq.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hco.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://jjn.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hhq.mhx1999.top

[R26] 命令替换
来源：http://iyk.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://fqf.xylfe.cn

[R27] 算术展开
来源：http://whv.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://tdc.wangshuangyany.cn

[R28] 浮点运算
来源：http://dfi.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://yal.c1oappe.top

[R29] 定义函数
来源：http://vcm.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qbt.sysykeji.top

[R30] 函数返回状态码
来源：http://wcu.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://fwg.shzxlz.cn

[R31] 局部变量
来源：http://fbu.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://cqw.yj20258.top

[R32] 参数个数校验
来源：http://waq.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ktv.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://pdh.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hor.jqgufenzy.top

[R34] 退出时清理
来源：http://xiq.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://cyk.snrcjt.cn

[R35] 后台执行并等待
来源：http://joe.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ded.aibaodan.cn

[R36] 并发执行多个任务
来源：http://bsz.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sim.svipenyu.cn

[R37] 把输出赋给变量
来源：http://spe.fanxiaobao.xyz

files=$(ls -1)
来源：http://fpd.xziqi.cn

[R38] 管道串联
来源：http://zwz.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://nut.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://jpx.xinyue.icu

cmd > out.log 2>&1
来源：http://qey.316326.xyz

[R40] 追加写日志
来源：http://buk.zhiwuduotai.top

echo "log" >> out.log
来源：http://dhz.epnwcf.com

[R41] 丢弃输出
来源：http://rmw.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://fsc.sysykeji.top

[R42] 输入重定向
来源：http://hee.yueranfly.top

wc -l < a.txt
来源：http://ypj.cdnleiting.top

[R43] 按名字查找文件
来源：http://jdz.yj20258.top

find . -name "*.log" -type f
来源：http://zfx.52xcode.cn

[R44] 按修改时间查找
来源：http://gta.ivvv.top

find . -mtime -7 -type f
来源：http://mlk.gzhubu.top

[R45] 批量删除
来源：http://gby.havefunace.top

find . -name "*.tmp" -delete
来源：http://msg.cashguo.top

[R46] 递归替换文件内容
来源：http://pmw.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jxz.uphjek.com

[R47] sed 单行替换
来源：http://wdo.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nfj.vehdjk.com

[R48] awk 取指定列
来源：http://mod.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://xmb.zhongyouzk.top

[R49] awk 带条件
来源：http://xew.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hqj.vehdjk.com

[R50] awk 求和
来源：http://hsk.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://bzk.svipenyu.cn

[R51] 排序去重取前几
来源：http://yae.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kfg.haohaochexian.top

[R52] 统计行数
来源：http://fvf.yj20258888.top

wc -l a.txt
来源：http://xvt.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://osb.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zwt.zhixingplan.top

[R54] 比较两个文件
来源：http://vrx.tanke756.top

diff a.txt b.txt
来源：http://maf.c1oappe.top

[R55] 压缩与解压
来源：http://hsz.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dvh.tianlin.xyz

[R56] 远程拷贝
来源：http://zsg.daxiang520.top

scp file user@host:/path/
来源：http://puy.gogol.net.cn

[R57] 远程执行命令
来源：http://hoa.yj20258.top

ssh user@host 'uptime'
来源：http://uzy.316326.xyz

[R58] 下载文件
来源：http://ujt.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hrc.wangdashe.top

[R59] 发 POST JSON
来源：http://wyr.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tbh.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://pfo.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odp.nanxuanxn.top

[R61] 磁盘占用
来源：http://kkq.fehbvm.com

df -h;  du -sh *
来源：http://qlm.ppjwa.cn

[R62] 找最占空间的文件
来源：http://ybv.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://iaj.jiagoushi.top

[R63] 内存与进程
来源：http://que.sufxvd.cn


<!-- 参考信息 -->