代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ozl.dashuyun.cn

[Q20] IN 列表
来源：http://wfq.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kfq.cucudq.cn

[Q21] 空值判断
来源：http://jji.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://beh.aizwys.cn

[Q22] 排序
来源：http://cah.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vyr.andypj.xyz

[Q23] 分页
来源：http://sui.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gdr.hcnkem.com

[Q24] 去重
来源：http://yjl.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://ytw.xylfe.cn

[Q25] 只取前 N 条
来源：http://ktm.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xqj.cdnleiting.top

[Q26] 计数
来源：http://cxw.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://kfq.hesvh.cn

[Q27] 条件计数
来源：http://wda.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://egm.tianlin.xyz

[Q28] 求和与平均
来源：http://avj.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lge.cucudq.cn

[Q29] 最大最小值
来源：http://haf.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cnw.wangshuangyany.cn

[Q30] 分组统计
来源：http://tqk.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://usa.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://kfa.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gov.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://mua.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eze.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ayp.redwolf501.top

[Q33] 多列分组
来源：http://frc.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://asi.fehbvm.com

[Q34] 每组取第一条
来源：http://tjz.guannengcc.top

SELECT * FROM (
来源：http://kvs.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nvm.jinqigufen.top

) t WHERE rn = 1;
来源：http://kum.c1oappe.top

[Q35] 内连接
来源：http://fxw.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wqb.hnxiangtu.top

[Q36] 左连接
来源：http://myf.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oba.yj202588.top

[Q37] 右连接
来源：http://asr.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mjk.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://dqn.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ixb.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://zou.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xrb.tianlin.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rpu.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mnw.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gvv.zhoulong.xyz

[Q41] 多表连接
来源：http://ekw.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://gpf.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://xls.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://ksv.yonumen.top

[Q42] 连接条件附加过滤
来源：http://bpw.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://utu.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rnl.zhijiandao.cn

[Q43] 标量子查询
来源：http://vvs.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bws.hysaishi.cn

[Q44] IN 子查询
来源：http://qzf.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yho.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://emg.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cxv.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://rjz.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owm.c1oappe.top

[Q47] 与平均值比较
来源：http://tot.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jtb.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://vsl.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://saj.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://wvb.hongshengwenyu.top

[Q49] 更新单行
来源：http://bsv.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yku.jinghuilouyu.cn

[Q50] 批量更新
来源：http://fnc.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cjo.hnqzz.top

[Q51] 用子查询更新
来源：http://scy.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iru.xuanzx.com

[Q52] 删除指定行
来源：http://npa.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://xhj.xinyue.icu

[Q53] 按条件删除
来源：http://yga.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dyg.fktsv.cn

[Q54] 清空表
来源：http://yuc.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://dil.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://vwn.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://shz.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://fuh.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ttk.ywan-chungtsiang.top

[Q57] 行号
来源：http://qwh.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zhq.bjfxy.top

[Q58] 累计求和
来源：http://kip.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dhd.yangfankeji.com

[Q59] 分组内累计
来源：http://wpl.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wjv.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://ykj.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lav.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qoj.hammf.cn

[Q61] 移动平均
来源：http://gjh.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://akw.tianlin.xyz

[Q62] 分组占比
来源：http://qxb.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hxa.cdnleiting.top

[Q63] 开启事务
来源：http://tgj.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hie.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://rlh.zhoulong.xyz

COMMIT;
来源：http://vrw.wangshuangyany.cn

[Q65] 回滚事务
来源：http://wvi.shuidangran.top

ROLLBACK;
来源：http://urc.gogol.net.cn

[Q66] 行锁查询
来源：http://nuu.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hjm.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://uue.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ugp.jinqigfzy.top

[Q68] 保存点
来源：http://res.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://vuk.daria6918.cn

ROLLBACK TO sp1;
来源：http://wxm.smart0.xyz

[Q69] 查看执行计划
来源：http://qrv.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ned.fktsv.cn

[Q70] 更新统计信息
来源：http://xpo.tanke756.top

ANALYZE TABLE users;
来源：http://abx.xylfe.cn

[Q71] 查看建表语句
来源：http://ryt.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jay.sjlbkw.cn

[Q72] 查看索引
来源：http://kbs.birdmap.top

SHOW INDEX FROM users;
来源：http://aiu.hywenlv.cn

[Q73] 查看表状态
来源：http://lod.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://osi.cashguo.top

[Q74] 强制使用索引
来源：http://aht.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qwa.redwolf501.top

[Q75] 日期格式化
来源：http://rps.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qhg.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://krn.jiagoushi.top

[Q76] 按天统计
来源：http://tsn.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://obo.9152youxi.cn

[Q77] 时间加减
来源：http://hem.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rjz.cheryme.top

[Q78] 当前时间
来源：http://vfh.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kkb.yj20258888.top

[Q79] 字符串拼接
来源：http://piz.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://viu.cqqwz.cn

[Q80] 字符串截取
来源：http://hrb.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wef.chenjidiqi.icu

[Q81] 字符串替换
来源：http://jbu.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nog.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://zzn.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gbg.gzhubu.top

[Q83] 大小写转换
来源：http://jjy.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dmk.shzxlz.cn

[Q84] 去除首尾空格
来源：http://tiq.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://utb.chenlongwang.top

[Q85] 数值取整
来源：http://keb.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mwr.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://teq.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hbd.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://mim.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xtc.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://tpd.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hfj.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://esw.mhx1999.top

[Q89] 判断表是否存在
来源：http://hcf.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hgb.zhengqikj.top

[Q90] 生成序号列
来源：http://ank.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hka.nanxinkj.top

================================================================================
来源：http://vnc.zhoulong.xyz

R. Bash 专题
来源：http://waa.birdmap.top

================================================================================
来源：http://rhm.birdmap.top

[R01] shebang 与严格模式
来源：http://ncb.zhengqikj.top

#!/usr/bin/env bash
来源：http://cvy.jinqigufen.top

set -euo pipefail
来源：http://tsa.sweek.top

[R02] 变量赋值与使用
来源：http://cgv.316326.xyz

name="Tom"; echo "$name"
来源：http://xid.gzhubu.top

[R03] 只读变量
来源：http://hhn.zhiwuduotai.top

readonly PI=3.14
来源：http://wfr.zhijiandao.cn

[R04] 位置参数
来源：http://hmv.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vip.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://tiw.zhoulong.xyz

name="${1:-default}"
来源：http://qxn.zycfv.cn

[R06] 判断命令是否存在
来源：http://qvf.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xrn.yueranfly.top

[R07] if 判断文件
来源：http://soa.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xdj.yvedp.cn

[R08] 数值比较
来源：http://rhq.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vdv.gaohongyu789.top

[R09] 字符串比较
来源：http://akf.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dya.smart0.xyz

[R10] 正则匹配
来源：http://ohz.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hdo.jinqigfzy.top

[R11] case 多分支
来源：http://iol.yongpay.top

case "$1" in
来源：http://qdw.meibo888.top

start) echo "启动" ;;
来源：http://wto.haohaochexian.top

stop)  echo "停止" ;;
来源：http://fbw.nwbrower.top

*)     echo "未知命令" ;;
来源：http://hka.yfazqb.com

esac
来源：http://ciu.bjfxy.top

[R12] for 遍历文件
来源：http://wyd.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://mnk.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://jas.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://iiu.tianlin.xyz

[R14] C 风格 for
来源：http://rrw.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xtj.yj20258888.top

[R15] while 逐行读文件
来源：http://kvb.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ktn.chenlongwang.top

[R16] until 等待条件
来源：http://msg.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aki.nanxuanxn.top

[R17] 数组定义与取值
来源：http://yte.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hjr.zhongyouzk.top

[R18] 遍历数组
来源：http://qgd.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lxm.sysykeji.top

[R19] 数组长度
来源：http://qdi.ydjk.org.cn

echo "${#arr[@]}"
来源：http://lhc.fehbvm.com

[R20] 关联数组（字典）
来源：http://vlh.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://atv.daria6918.cn

[R21] 字符串长度
来源：http://poz.sxryk.cn

echo "${#s}"
来源：http://esb.zhengqikj.top

[R22] 截取子串
来源：http://rcn.jinqigfzy.top

echo "${s:0:5}"
来源：http://bbp.hnqzz.top

[R23] 字符串替换
来源：http://ycz.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ary.zhiwuduotai.top

[R24] 大小写转换
来源：http://qnc.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wkf.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://jyu.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yiw.cqqwz.cn

[R26] 命令替换
来源：http://dxq.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://riy.sysykeji.top

[R27] 算术展开
来源：http://fbe.yj20258888.top

echo $((1 + 2 * 3))
来源：http://ygw.yj20258888.top

[R28] 浮点运算
来源：http://ydm.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://dvb.fanxiaobao.xyz

[R29] 定义函数
来源：http://umm.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpp.ctjpmb.com

[R30] 函数返回状态码
来源：http://zfb.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://gzy.birdmap.top

[R31] 局部变量
来源：http://ffq.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://syh.xuanzx.com

[R32] 参数个数校验
来源：http://vkj.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ynn.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://xwy.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dfy.jinqigfzy.top

[R34] 退出时清理
来源：http://sxx.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://zac.tarul.cn

[R35] 后台执行并等待
来源：http://zxt.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ipk.andypj.xyz

[R36] 并发执行多个任务
来源：http://pte.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zfo.guowangkeji.top

[R37] 把输出赋给变量
来源：http://yhi.yuxming.cn

files=$(ls -1)
来源：http://ngi.chenzaomai.com

[R38] 管道串联
来源：http://fnp.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://fcl.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://pie.xinyue.icu

cmd > out.log 2>&1
来源：http://esj.xziqi.cn

[R40] 追加写日志
来源：http://del.wangshuangyany.cn

echo "log" >> out.log
来源：http://ivy.0kj1m.cn

[R41] 丢弃输出
来源：http://qaa.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://xvu.xylfe.cn

[R42] 输入重定向
来源：http://urn.chenzaomai.com

wc -l < a.txt
来源：http://zln.iojbl.cn

[R43] 按名字查找文件
来源：http://bup.cdnleiting.top

find . -name "*.log" -type f
来源：http://ytl.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://fcv.ybcxt.top

find . -mtime -7 -type f
来源：http://cyt.fktsv.cn

[R45] 批量删除
来源：http://jhl.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://rjq.cheryme.top

[R46] 递归替换文件内容
来源：http://gvk.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://piw.sufxvd.cn

[R47] sed 单行替换
来源：http://gjt.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://qhi.yonumen.top

[R48] awk 取指定列
来源：http://yfw.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://qnm.sjlbkw.cn

[R49] awk 带条件
来源：http://luj.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://frm.cdnleiting.top

[R50] awk 求和
来源：http://vly.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gas.yj20258888.top

[R51] 排序去重取前几
来源：http://hbu.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ibj.yonumen.top

[R52] 统计行数
来源：http://uog.mhx1999.top

wc -l a.txt
来源：http://lrd.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://yph.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dlg.pengpengdd.cyou

[R54] 比较两个文件
来源：http://glm.sxryk.cn

diff a.txt b.txt
来源：http://lxr.pycfn.com

[R55] 压缩与解压
来源：http://fce.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xkm.hywenlv.cn

[R56] 远程拷贝
来源：http://sjc.jinqigufen.top

scp file user@host:/path/
来源：http://frd.guowangkeji.top

[R57] 远程执行命令
来源：http://dfe.yuxming.cn

ssh user@host 'uptime'
来源：http://siz.bjfxy.top

[R58] 下载文件
来源：http://nii.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dck.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://eae.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://swy.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://zgs.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pwc.xinyue.icu

[R61] 磁盘占用
来源：http://gdj.zhengqikj.top

df -h;  du -sh *
来源：http://nld.zdqjudy.top

[R62] 找最占空间的文件
来源：http://plk.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://sun.shangyingyoupin.top

[R63] 内存与进程
来源：http://tee.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://wov.chenjidiqi.icu

[R64] 结束进程
来源：http://ksz.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://gnq.chenlongwang.top

[R65] 查看端口占用
来源：http://wzh.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hsh.yj20258888.top

[R66] 定时任务
来源：http://grf.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://hxs.sxryk.cn

[R67] 生成随机十六进制串
来源：http://hoq.redwolf501.top

openssl rand -hex 16
来源：http://wga.hywenlv.cn

[R68] 计算文件校验值
来源：http://fnd.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://ack.yueranfly.top

[R69] 生成随机密码
来源：http://cgj.jinyuanbaomall.cn


<!-- 参考信息 -->