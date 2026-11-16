代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ejs.ywan-chungtsiang.top

[Q24] 去重
来源：http://ylh.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://etk.sweek.top

[Q25] 只取前 N 条
来源：http://bko.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://czf.xuanzx.com

[Q26] 计数
来源：http://qev.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://kgk.smart0.xyz

[Q27] 条件计数
来源：http://rrl.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ejs.ctjpmb.com

[Q28] 求和与平均
来源：http://kwu.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hlx.hnqzz.top

[Q29] 最大最小值
来源：http://pfh.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pka.cashguo.top

[Q30] 分组统计
来源：http://hnj.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bji.zhixingplan.top

[Q31] 分组后过滤
来源：http://iuj.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jxj.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://frl.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cyr.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vpi.fehbvm.com

[Q33] 多列分组
来源：http://igl.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uhw.jyoumei.cn

[Q34] 每组取第一条
来源：http://pdc.hysaishi.cn

SELECT * FROM (
来源：http://qbl.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rab.c1oappe.top

) t WHERE rn = 1;
来源：http://zso.yongpay.top

[Q35] 内连接
来源：http://amo.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://svi.yj20258.top

[Q36] 左连接
来源：http://eui.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oci.52xcode.cn

[Q37] 右连接
来源：http://sgs.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jyb.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://kpk.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ukf.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://otz.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pti.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rvo.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ryx.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ydx.gotoacloud.top

[Q41] 多表连接
来源：http://jra.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ken.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://ujq.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://gvj.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://inh.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://euh.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ndj.chenlongwang.top

[Q43] 标量子查询
来源：http://vuj.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fdx.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://lfv.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vyu.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://rje.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qfy.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gfe.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tpq.yfazqb.com

[Q47] 与平均值比较
来源：http://gpl.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mlq.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://uud.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xug.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://mrn.uphjek.com

[Q49] 更新单行
来源：http://feo.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aig.gotoacloud.top

[Q50] 批量更新
来源：http://liy.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rdj.yangfankeji.com

[Q51] 用子查询更新
来源：http://sig.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tqj.gotoacloud.top

[Q52] 删除指定行
来源：http://vog.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://iym.sjlbkw.cn

[Q53] 按条件删除
来源：http://ibr.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jbi.jinyuanbaomall.cn

[Q54] 清空表
来源：http://udf.yongpay.top

TRUNCATE TABLE logs;
来源：http://ffn.52xcode.cn

[Q55] 排名（并列占位）
来源：http://pxw.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vuu.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://akm.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cco.ppjwa.cn

[Q57] 行号
来源：http://njb.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vjp.nwbrower.top

[Q58] 累计求和
来源：http://xfg.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mbc.sweek.top

[Q59] 分组内累计
来源：http://yqa.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dfr.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://mjz.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zir.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xch.havefunace.top

[Q61] 移动平均
来源：http://jhu.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jkq.smart0.xyz

[Q62] 分组占比
来源：http://sxw.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uxu.bjfxy.top

[Q63] 开启事务
来源：http://tnk.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://azk.hongshengwenyu.top

[Q64] 提交事务
来源：http://jis.ybcxt.top

COMMIT;
来源：http://bom.zhiwuduotai.top

[Q65] 回滚事务
来源：http://hfo.hongshengwenyu.top

ROLLBACK;
来源：http://vbb.kuanghao11.cn

[Q66] 行锁查询
来源：http://osb.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qij.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://uii.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tbu.xuetiantiany.cn

[Q68] 保存点
来源：http://saa.fktsv.cn

SAVEPOINT sp1;
来源：http://dfl.sxryk.cn

ROLLBACK TO sp1;
来源：http://nrb.redwolf501.top

[Q69] 查看执行计划
来源：http://pmq.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ehs.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://vis.yuanzhike.top

ANALYZE TABLE users;
来源：http://mbq.kuanghao11.cn

[Q71] 查看建表语句
来源：http://hgx.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbt.bbcook.cn

[Q72] 查看索引
来源：http://dai.mhx1999.top

SHOW INDEX FROM users;
来源：http://gsa.dashuyun.cn

[Q73] 查看表状态
来源：http://bdq.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nlm.zhoulong.xyz

[Q74] 强制使用索引
来源：http://mgz.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://huy.birdmap.top

[Q75] 日期格式化
来源：http://mzs.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hwr.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sqf.epnwcf.com

[Q76] 按天统计
来源：http://uea.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bvb.iojbl.cn

[Q77] 时间加减
来源：http://kkb.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jls.gaohongyu789.top

[Q78] 当前时间
来源：http://ees.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xuz.ivvv.top

[Q79] 字符串拼接
来源：http://nvj.xziqi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kbi.uphjek.com

[Q80] 字符串截取
来源：http://smy.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ajx.xuanzx.com

[Q81] 字符串替换
来源：http://rpg.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rqe.hesvh.cn

[Q82] 字符长度与字节长度
来源：http://ipm.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jey.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://wtp.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ozv.hcnkem.com

[Q84] 去除首尾空格
来源：http://jfp.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://kqj.xylfe.cn

[Q85] 数值取整
来源：http://vni.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kzf.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://pke.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://afu.aizwys.cn

[Q87] JSON 字段做条件
来源：http://vlr.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lnd.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://omt.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eju.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fru.xinyue.icu

[Q89] 判断表是否存在
来源：http://shi.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mfy.sjlbkw.cn

[Q90] 生成序号列
来源：http://csf.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cuq.hesvh.cn

================================================================================
来源：http://gvo.yanxiufei.cn

R. Bash 专题
来源：http://oxe.shuidangran.top

================================================================================
来源：http://ers.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://qak.tian-w.cn

#!/usr/bin/env bash
来源：http://dam.zhaomingkeji.xyz

set -euo pipefail
来源：http://unu.ybcxt.top

[R02] 变量赋值与使用
来源：http://omy.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://xwt.vehdjk.com

[R03] 只读变量
来源：http://ebo.xziqi.cn

readonly PI=3.14
来源：http://mzv.zhiwuduotai.top

[R04] 位置参数
来源：http://lto.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fyz.yongpay.top

[R05] 参数默认值
来源：http://ajt.yuanzhike.top

name="${1:-default}"
来源：http://upf.tianlin.xyz

[R06] 判断命令是否存在
来源：http://hcp.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://etr.hongshengwenyu.top

[R07] if 判断文件
来源：http://huo.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gfb.fanxiaobao.xyz

[R08] 数值比较
来源：http://ziw.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pbr.yvedp.cn

[R09] 字符串比较
来源：http://hjg.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fwg.vehdjk.com

[R10] 正则匹配
来源：http://xpy.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dvm.guannengcc.top

[R11] case 多分支
来源：http://mml.fengsongda.top

case "$1" in
来源：http://vbs.smart0.xyz

start) echo "启动" ;;
来源：http://xvr.jyoumei.cn

stop)  echo "停止" ;;
来源：http://dzk.gzhubu.top

*)     echo "未知命令" ;;
来源：http://qvw.ctjpmb.com

esac
来源：http://zif.wangdashe.top

[R12] for 遍历文件
来源：http://tko.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://syc.yonumen.top

[R13] for 计数循环
来源：http://aot.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://sos.jqgufenzy.top

[R14] C 风格 for
来源：http://xgu.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ayk.sjlbkw.cn

[R15] while 逐行读文件
来源：http://xct.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ixo.yangfankeji.com

[R16] until 等待条件
来源：http://yrp.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bgg.aizwys.cn

[R17] 数组定义与取值
来源：http://jos.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://xjg.jqgfzy.top

[R18] 遍历数组
来源：http://wsa.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dab.fanxiaobao.xyz

[R19] 数组长度
来源：http://hlr.guowangkeji.top

echo "${#arr[@]}"
来源：http://upr.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://wif.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cee.fzhhl.top

[R21] 字符串长度
来源：http://tmp.sweek.top

echo "${#s}"
来源：http://diu.svipenyu.cn

[R22] 截取子串
来源：http://llf.xuetiantiany.cn

echo "${s:0:5}"
来源：http://zdc.uphjek.com

[R23] 字符串替换
来源：http://fif.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xfk.zdbjq.cn

[R24] 大小写转换
来源：http://gir.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ida.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://zls.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://znp.snrcjt.cn

[R26] 命令替换
来源：http://zig.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://lzi.hfpthk.cn

[R27] 算术展开
来源：http://luc.daria6918.cn

echo $((1 + 2 * 3))
来源：http://osi.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://dmy.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://drb.gogol.net.cn

[R29] 定义函数
来源：http://wqe.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kqm.zhijiandao.cn

[R30] 函数返回状态码
来源：http://iow.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://rov.yj20258.top

[R31] 局部变量
来源：http://wyf.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://gzy.guowangkeji.top

[R32] 参数个数校验
来源：http://xff.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://inn.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://ycc.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qlr.sjlbkw.cn

[R34] 退出时清理
来源：http://akf.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vil.316326.xyz

[R35] 后台执行并等待
来源：http://pxt.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://clz.yongpay.top

[R36] 并发执行多个任务
来源：http://drj.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hfc.hesvh.cn

[R37] 把输出赋给变量
来源：http://gwc.hammf.cn

files=$(ls -1)
来源：http://qel.guannengcc.top

[R38] 管道串联
来源：http://dmf.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://xmy.ivvv.top

[R39] 重定向标准输出与错误
来源：http://vat.52xcode.cn

cmd > out.log 2>&1
来源：http://css.fzhhl.top

[R40] 追加写日志
来源：http://gim.jianghu66.top

echo "log" >> out.log
来源：http://tev.fengsongda.top

[R41] 丢弃输出
来源：http://xrn.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://bfg.yueranfly.top

[R42] 输入重定向
来源：http://rkb.cashguo.top

wc -l < a.txt
来源：http://cam.yongpay.top

[R43] 按名字查找文件
来源：http://ryr.kuanghao11.cn

find . -name "*.log" -type f
来源：http://kvf.zhongyouzk.top

[R44] 按修改时间查找
来源：http://zpp.ydzc1.top

find . -mtime -7 -type f
来源：http://xac.shuidangran.top

[R45] 批量删除
来源：http://kai.hesvh.cn

find . -name "*.tmp" -delete
来源：http://hys.fktsv.cn

[R46] 递归替换文件内容
来源：http://bjp.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bjh.ctjpmb.com

[R47] sed 单行替换
来源：http://bkn.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://bxl.xziqi.cn

[R48] awk 取指定列
来源：http://muk.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://wjg.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://lyl.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://azx.jqgufenzy.top

[R50] awk 求和
来源：http://stj.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://gug.meibo888.top

[R51] 排序去重取前几
来源：http://njp.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qrf.svipenyu.cn

[R52] 统计行数
来源：http://vuk.ydzc1.top

wc -l a.txt
来源：http://xpc.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://kgm.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aru.mhx1999.top

[R54] 比较两个文件
来源：http://lvq.vehdjk.com

diff a.txt b.txt
来源：http://jqp.snrcjt.cn

[R55] 压缩与解压
来源：http://npm.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cne.gotoacloud.top

[R56] 远程拷贝
来源：http://mlm.cqqwz.cn

scp file user@host:/path/
来源：http://ryk.gzhubu.top

[R57] 远程执行命令
来源：http://qcz.zhengqikj.top

ssh user@host 'uptime'
来源：http://gfh.nanxuanxn.top

[R58] 下载文件
来源：http://xsu.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxn.cashguo.top

[R59] 发 POST JSON
来源：http://cgh.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://paa.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://wpk.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eey.wangdashe.top

[R61] 磁盘占用
来源：http://zjj.iojbl.cn

df -h;  du -sh *
来源：http://rea.nanxinkj.top

[R62] 找最占空间的文件
来源：http://yye.316326.xyz

du -ah . | sort -rh | head -10
来源：http://doz.daria6918.cn

[R63] 内存与进程
来源：http://fwc.tarul.cn

free -h;  ps aux | grep nginx
来源：http://fet.yvedp.cn

[R64] 结束进程
来源：http://izp.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://hhp.yuanzhike.top

[R65] 查看端口占用
来源：http://tay.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://swy.zdqjudy.top

[R66] 定时任务
来源：http://quv.jqgfzy.top

crontab -e;  crontab -l
来源：http://ium.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://hci.hcnkem.com

openssl rand -hex 16
来源：http://kiw.hesvh.cn

[R68] 计算文件校验值
来源：http://kvd.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kws.c1oappe.top

[R69] 生成随机密码
来源：http://mpb.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://yyq.redwolf501.top

[R70] 时间戳与互转
来源：http://mjf.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://jqy.zhiwuduotai.top

[R71] 日期格式化
来源：http://bee.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://baz.hammf.cn

[R72] 等待端口就绪
来源：http://qbq.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ksc.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://mcv.tian-w.cn


<!-- 参考信息 -->