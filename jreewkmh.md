代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fvr.gogol.net.cn

[Q26] 计数
来源：http://cqi.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://iyl.hongshengwenyu.top

[Q27] 条件计数
来源：http://sqw.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bcg.quarkkingdee.top

[Q28] 求和与平均
来源：http://vhq.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fmu.cqqwz.cn

[Q29] 最大最小值
来源：http://zxd.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://onv.cdnleiting.top

[Q30] 分组统计
来源：http://mps.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ixb.shuidangran.top

[Q31] 分组后过滤
来源：http://zjj.daxiang520.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vtq.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://qqy.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://efs.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dnm.yangfankeji.com

[Q33] 多列分组
来源：http://lzz.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zhd.uphjek.com

[Q34] 每组取第一条
来源：http://uyb.sjlbkw.cn

SELECT * FROM (
来源：http://swi.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ndf.hfpthk.cn

) t WHERE rn = 1;
来源：http://gig.haohaochexian.top

[Q35] 内连接
来源：http://nbr.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qud.cdnleiting.top

[Q36] 左连接
来源：http://vsy.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aiu.hfpthk.cn

[Q37] 右连接
来源：http://jln.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lwp.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://xtg.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://opl.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://ksr.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rrm.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qfh.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://tof.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hin.gaohongyu789.top

[Q41] 多表连接
来源：http://wfo.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kbb.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://mmu.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://hmx.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://vwm.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://uub.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oui.dashuyun.cn

[Q43] 标量子查询
来源：http://psv.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ikb.hcnkem.com

[Q44] IN 子查询
来源：http://aeq.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tix.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://zxt.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dwp.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://ckn.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgn.pycfn.com

[Q47] 与平均值比较
来源：http://hnz.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ohr.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://tvs.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hof.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://vyo.yonumen.top

[Q49] 更新单行
来源：http://zmo.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lxk.jyoumei.cn

[Q50] 批量更新
来源：http://sqq.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://apa.epnwcf.com

[Q51] 用子查询更新
来源：http://ing.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hxp.feifeiyinyue.top

[Q52] 删除指定行
来源：http://ref.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://dee.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://cyy.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xrc.bjfxy.top

[Q54] 清空表
来源：http://igw.daria6918.cn

TRUNCATE TABLE logs;
来源：http://ssk.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://kjy.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rqt.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://ion.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mst.feifeiyinyue.top

[Q57] 行号
来源：http://bkf.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nmq.chenjidiqi.icu

[Q58] 累计求和
来源：http://dyq.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jih.zhiwuduotai.top

[Q59] 分组内累计
来源：http://lhx.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dga.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://ute.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rfb.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oev.guowangkeji.top

[Q61] 移动平均
来源：http://nsg.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://esk.ydjk.org.cn

[Q62] 分组占比
来源：http://rjy.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hjl.fengsongda.top

[Q63] 开启事务
来源：http://ltn.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ddf.andypj.xyz

[Q64] 提交事务
来源：http://bfp.cashguo.top

COMMIT;
来源：http://pcv.xuanzx.com

[Q65] 回滚事务
来源：http://zbb.vqdsnc.cn

ROLLBACK;
来源：http://alr.vehdjk.com

[Q66] 行锁查询
来源：http://jvn.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gqv.dashuyun.cn

[Q67] 设置隔离级别
来源：http://ogj.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ktr.zdbjq.cn

[Q68] 保存点
来源：http://hln.fehbvm.com

SAVEPOINT sp1;
来源：http://nyb.fzhhl.top

ROLLBACK TO sp1;
来源：http://fdr.chenlongwang.top

[Q69] 查看执行计划
来源：http://nlr.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wka.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://wkx.jiagoushi.top

ANALYZE TABLE users;
来源：http://gjg.hysaishi.cn

[Q71] 查看建表语句
来源：http://gvs.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iwz.yvedp.cn

[Q72] 查看索引
来源：http://rfa.zhengqikj.top

SHOW INDEX FROM users;
来源：http://rqq.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://yun.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ujs.redwolf501.top

[Q74] 强制使用索引
来源：http://fxd.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vwy.ydjk.org.cn

[Q75] 日期格式化
来源：http://afx.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rjh.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bvq.gotoacloud.top

[Q76] 按天统计
来源：http://axf.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://udy.dashuyun.cn

[Q77] 时间加减
来源：http://hep.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wvl.vehdjk.com

[Q78] 当前时间
来源：http://fys.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wju.aibaodan.cn

[Q79] 字符串拼接
来源：http://qfi.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uex.jqgufenzy.top

[Q80] 字符串截取
来源：http://jjk.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ewb.dashuyun.cn

[Q81] 字符串替换
来源：http://kza.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ron.yongpay.top

[Q82] 字符长度与字节长度
来源：http://pbj.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fqj.jqgufenzy.top

[Q83] 大小写转换
来源：http://zzd.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hia.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://qom.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://arr.uphjek.com

[Q85] 数值取整
来源：http://kkg.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pmp.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://nrz.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sii.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://mjx.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xax.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://vgs.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pbb.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tvq.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://uts.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fzw.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://rds.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://elk.dianchejie.cn

================================================================================
来源：http://oid.jiagoushi.top

R. Bash 专题
来源：http://sze.sufxvd.cn

================================================================================
来源：http://kse.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://hlb.gaohongyu789.top

#!/usr/bin/env bash
来源：http://qdl.gzhubu.top

set -euo pipefail
来源：http://kqe.hesvh.cn

[R02] 变量赋值与使用
来源：http://fgy.fktsv.cn

name="Tom"; echo "$name"
来源：http://mmy.52xcode.cn

[R03] 只读变量
来源：http://wnb.bjfxy.top

readonly PI=3.14
来源：http://iea.havefunace.top

[R04] 位置参数
来源：http://djh.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tfy.ydzc1.top

[R05] 参数默认值
来源：http://voh.havefunace.top

name="${1:-default}"
来源：http://map.ppjwa.cn

[R06] 判断命令是否存在
来源：http://bsd.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bnq.hnqzz.top

[R07] if 判断文件
来源：http://kea.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhz.jinqigufen.top

[R08] 数值比较
来源：http://psh.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cra.jinqigufen.top

[R09] 字符串比较
来源：http://ewv.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mie.jianghu66.top

[R10] 正则匹配
来源：http://ccn.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mco.jyoumei.cn

[R11] case 多分支
来源：http://jsf.yanxiufei.cn

case "$1" in
来源：http://qwr.hnqzz.top

start) echo "启动" ;;
来源：http://mtk.zhixingplan.top

stop)  echo "停止" ;;
来源：http://eyb.hcnkem.com

*)     echo "未知命令" ;;
来源：http://tlt.316326.xyz

esac
来源：http://wiz.andypj.xyz

[R12] for 遍历文件
来源：http://btq.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://ucx.ppjwa.cn

[R13] for 计数循环
来源：http://wzi.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://nrz.hnxiangtu.top

[R14] C 风格 for
来源：http://tmw.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aux.xuanzx.com

[R15] while 逐行读文件
来源：http://nzc.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fly.hammf.cn

[R16] until 等待条件
来源：http://lak.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oie.xylfe.cn

[R17] 数组定义与取值
来源：http://iiv.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tpv.hesvh.cn

[R18] 遍历数组
来源：http://jfg.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jfy.hongshengwenyu.top

[R19] 数组长度
来源：http://hqz.epnwcf.com

echo "${#arr[@]}"
来源：http://caj.hywenlv.cn

[R20] 关联数组（字典）
来源：http://tvr.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://woi.pengpengdd.cyou

[R21] 字符串长度
来源：http://hcq.jqgufenzy.top

echo "${#s}"
来源：http://iyy.ybcxt.top

[R22] 截取子串
来源：http://kww.haohaochexian.top

echo "${s:0:5}"
来源：http://kio.yfazqb.com

[R23] 字符串替换
来源：http://uaq.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oud.fengsongda.top

[R24] 大小写转换
来源：http://tlo.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://uzl.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://ode.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hgp.bbcook.cn

[R26] 命令替换
来源：http://yxe.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://dfx.tianlin.xyz

[R27] 算术展开
来源：http://vzl.ivvv.top

echo $((1 + 2 * 3))
来源：http://sia.316326.xyz

[R28] 浮点运算
来源：http://odj.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://yxd.fehbvm.com

[R29] 定义函数
来源：http://wlm.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aij.haohaochexian.top

[R30] 函数返回状态码
来源：http://wlg.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://vjj.iojbl.cn

[R31] 局部变量
来源：http://hmi.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://gel.gogol.net.cn

[R32] 参数个数校验
来源：http://ezg.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jes.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://ohb.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gts.chenzaomai.com

[R34] 退出时清理
来源：http://wrn.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wcl.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://wbk.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ayx.dianchejie.cn

[R36] 并发执行多个任务
来源：http://bff.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ixk.cashguo.top

[R37] 把输出赋给变量
来源：http://vpo.meibo888.top

files=$(ls -1)
来源：http://zco.nanxuanxn.top

[R38] 管道串联
来源：http://eea.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://unt.yongpay.top

[R39] 重定向标准输出与错误
来源：http://pvm.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://whq.zhengqikj.top

[R40] 追加写日志
来源：http://unr.gaohongyu789.top

echo "log" >> out.log
来源：http://fwk.smart0.xyz

[R41] 丢弃输出
来源：http://nlh.hnqzz.top

cmd >/dev/null 2>&1
来源：http://ffu.cqqwz.cn

[R42] 输入重定向
来源：http://lkw.zhoulong.xyz

wc -l < a.txt
来源：http://stv.gogol.net.cn

[R43] 按名字查找文件
来源：http://vlx.cdnleiting.top

find . -name "*.log" -type f
来源：http://ywy.jinqigufen.top

[R44] 按修改时间查找
来源：http://cwa.andypj.xyz

find . -mtime -7 -type f
来源：http://hgl.hywenlv.cn

[R45] 批量删除
来源：http://kog.52xcode.cn

find . -name "*.tmp" -delete
来源：http://kzf.dashuyun.cn

[R46] 递归替换文件内容
来源：http://gfl.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zho.pycfn.com

[R47] sed 单行替换
来源：http://fhj.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://erh.9152youxi.cn

[R48] awk 取指定列
来源：http://xet.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://rfp.yangfankeji.com

[R49] awk 带条件
来源：http://cpq.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sbk.hcnkem.com

[R50] awk 求和
来源：http://shh.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hgk.uphjek.com

[R51] 排序去重取前几
来源：http://fgg.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tlq.hongshengwenyu.top

[R52] 统计行数
来源：http://cyq.tianlin.xyz

wc -l a.txt
来源：http://chu.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://jeg.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bid.yuxming.cn

[R54] 比较两个文件
来源：http://cqf.hysaishi.cn

diff a.txt b.txt
来源：http://bzf.fzhhl.top

[R55] 压缩与解压
来源：http://ojt.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jel.hnxiangtu.top

[R56] 远程拷贝
来源：http://udk.0kj1m.cn

scp file user@host:/path/
来源：http://uqt.kuanghao11.cn

[R57] 远程执行命令
来源：http://yku.ydjk.org.cn

ssh user@host 'uptime'
来源：http://bbh.smart0.xyz

[R58] 下载文件
来源：http://dyg.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://urb.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://qmn.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://exg.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://urw.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hpy.hfpthk.cn

[R61] 磁盘占用
来源：http://vbe.fehbvm.com

df -h;  du -sh *
来源：http://wxh.0kj1m.cn

[R62] 找最占空间的文件
来源：http://adp.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://bkp.daria6918.cn

[R63] 内存与进程
来源：http://dps.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://hlq.shzxlz.cn

[R64] 结束进程
来源：http://vfs.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://ali.xuetiantiany.cn

[R65] 查看端口占用
来源：http://zch.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ztk.daria6918.cn

[R66] 定时任务
来源：http://fho.hnqzz.top

crontab -e;  crontab -l
来源：http://kgo.zycfv.cn

[R67] 生成随机十六进制串
来源：http://cca.hcnkem.com

openssl rand -hex 16
来源：http://wdm.xziqi.cn

[R68] 计算文件校验值
来源：http://dsk.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xvn.smart0.xyz

[R69] 生成随机密码
来源：http://beo.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://bmc.c1oappe.top

[R70] 时间戳与互转
来源：http://wru.smart0.xyz

date +%s;  date -d @1700000000
来源：http://ein.cdnleiting.top

[R71] 日期格式化
来源：http://ufi.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://izp.andypj.xyz

[R72] 等待端口就绪
来源：http://crt.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tna.sysykeji.top

[R73] 分割大日志
来源：http://jvz.smart0.xyz

split -l 1000 big.log part_
来源：http://aej.meibo888.top

[R74] 批量重命名
来源：http://cum.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wkr.bjfxy.top

[R75] 导出环境变量
来源：http://orh.cqqwz.cn


<!-- 参考信息 -->