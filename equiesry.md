代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wzk.birdmap.top

[Q32] 分组拼接字符串
来源：http://zms.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bus.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kdt.hysaishi.cn

[Q33] 多列分组
来源：http://fsw.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wgw.zhengqikj.top

[Q34] 每组取第一条
来源：http://kuy.hnqzz.top

SELECT * FROM (
来源：http://oqd.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gfv.aibaodan.cn

) t WHERE rn = 1;
来源：http://bms.shanyushiyangtech.top

[Q35] 内连接
来源：http://oyq.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://urj.c1oappe.top

[Q36] 左连接
来源：http://web.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://plv.chenlongwang.top

[Q37] 右连接
来源：http://ali.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hgs.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cih.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mbb.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://bfz.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://wwi.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aso.jinghuilouyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qjl.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uuk.epnwcf.com

[Q41] 多表连接
来源：http://nsa.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ukt.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://fqj.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://isr.pycfn.com

[Q42] 连接条件附加过滤
来源：http://tly.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://koo.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zdp.yonumen.top

[Q43] 标量子查询
来源：http://bjb.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qki.vehdjk.com

[Q44] IN 子查询
来源：http://vgd.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://njj.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://jwu.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qrz.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fuj.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uat.aibaodan.cn

[Q47] 与平均值比较
来源：http://dhx.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zbz.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://jod.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kug.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://cpv.hfpthk.cn

[Q49] 更新单行
来源：http://neg.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vao.fanxiaobao.xyz

[Q50] 批量更新
来源：http://paf.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mpg.yvedp.cn

[Q51] 用子查询更新
来源：http://zqx.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xtg.andypj.xyz

[Q52] 删除指定行
来源：http://syi.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://ycs.redwolf501.top

[Q53] 按条件删除
来源：http://aby.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://umo.tanke756.top

[Q54] 清空表
来源：http://naw.xuanzx.com

TRUNCATE TABLE logs;
来源：http://rlg.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://iyw.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wsb.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://izh.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ttm.316326.xyz

[Q57] 行号
来源：http://hqc.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oca.0kj1m.cn

[Q58] 累计求和
来源：http://stw.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://onc.wangshuangyany.cn

[Q59] 分组内累计
来源：http://lgg.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehy.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://vgl.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rza.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nnr.epnwcf.com

[Q61] 移动平均
来源：http://gpg.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pdx.jqgfzy.top

[Q62] 分组占比
来源：http://mim.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mde.daxiang520.top

[Q63] 开启事务
来源：http://amq.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://bcm.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://iza.yfazqb.com

COMMIT;
来源：http://qbb.shzxlz.cn

[Q65] 回滚事务
来源：http://wvj.gaohongyu789.top

ROLLBACK;
来源：http://thn.fktsv.cn

[Q66] 行锁查询
来源：http://fwo.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fnx.yfazqb.com

[Q67] 设置隔离级别
来源：http://vlq.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oag.xuanzx.com

[Q68] 保存点
来源：http://baz.iojbl.cn

SAVEPOINT sp1;
来源：http://oez.fehbvm.com

ROLLBACK TO sp1;
来源：http://vxp.aizwys.cn

[Q69] 查看执行计划
来源：http://lxd.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pql.ppjwa.cn

[Q70] 更新统计信息
来源：http://edn.quarkkingdee.top

ANALYZE TABLE users;
来源：http://sec.xylfe.cn

[Q71] 查看建表语句
来源：http://pau.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rsq.fehbvm.com

[Q72] 查看索引
来源：http://fxc.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://puk.tarul.cn

[Q73] 查看表状态
来源：http://oos.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yrj.zhongyouzk.top

[Q74] 强制使用索引
来源：http://wai.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://awk.quarkkingdee.top

[Q75] 日期格式化
来源：http://ojb.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yps.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kbk.yfazqb.com

[Q76] 按天统计
来源：http://hqe.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ups.nanxinkj.top

[Q77] 时间加减
来源：http://sev.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rqr.zhongyouzk.top

[Q78] 当前时间
来源：http://ofl.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fnt.hfpthk.cn

[Q79] 字符串拼接
来源：http://oki.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dsx.zdbjq.cn

[Q80] 字符串截取
来源：http://mqq.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://amk.zdqjudy.top

[Q81] 字符串替换
来源：http://bhl.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://poe.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://krr.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wqn.yueranfly.top

[Q83] 大小写转换
来源：http://emt.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ciu.yuxming.cn

[Q84] 去除首尾空格
来源：http://qju.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://mpw.yuxming.cn

[Q85] 数值取整
来源：http://zfx.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://apo.tarul.cn

[Q86] 读取 JSON 字段
来源：http://omt.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://moh.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://uxa.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pmu.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://oem.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mby.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dog.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://sdy.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vrc.quarkkingdee.top

[Q90] 生成序号列
来源：http://yvy.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iog.hnqzz.top

================================================================================
来源：http://adz.svipenyu.cn

R. Bash 专题
来源：http://fqt.guannengcc.top

================================================================================
来源：http://nin.dashuyun.cn

[R01] shebang 与严格模式
来源：http://wmj.9152youxi.cn

#!/usr/bin/env bash
来源：http://uai.iojbl.cn

set -euo pipefail
来源：http://ghb.hysaishi.cn

[R02] 变量赋值与使用
来源：http://gyg.yvedp.cn

name="Tom"; echo "$name"
来源：http://srj.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://bol.yanxiufei.cn

readonly PI=3.14
来源：http://ucs.tianlin.xyz

[R04] 位置参数
来源：http://hdp.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wxr.quarkkingdee.top

[R05] 参数默认值
来源：http://lgt.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://ydt.aibaodan.cn

[R06] 判断命令是否存在
来源：http://mbj.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gnl.yuxming.cn

[R07] if 判断文件
来源：http://eyz.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sbs.ppjwa.cn

[R08] 数值比较
来源：http://rkg.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qgy.yuxming.cn

[R09] 字符串比较
来源：http://cfk.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dai.ydjk.org.cn

[R10] 正则匹配
来源：http://vyo.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ucs.birdmap.top

[R11] case 多分支
来源：http://pqo.cqqwz.cn

case "$1" in
来源：http://cbq.yongpay.top

start) echo "启动" ;;
来源：http://nfw.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://ood.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://zur.yangfankeji.com

esac
来源：http://vez.zhongyouzk.top

[R12] for 遍历文件
来源：http://apm.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://ost.jyoumei.cn

[R13] for 计数循环
来源：http://gwm.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://qpp.uphjek.com

[R14] C 风格 for
来源：http://ptk.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wew.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://drv.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zkq.shuidangran.top

[R16] until 等待条件
来源：http://hfc.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ays.yanxiufei.cn

[R17] 数组定义与取值
来源：http://mfh.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://ifi.zdqjudy.top

[R18] 遍历数组
来源：http://ebw.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wed.yj20258.top

[R19] 数组长度
来源：http://jbw.nanxinkj.top

echo "${#arr[@]}"
来源：http://czr.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://rrj.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tsx.zhongyouzk.top

[R21] 字符串长度
来源：http://eug.c1oappe.top

echo "${#s}"
来源：http://vek.sjlbkw.cn

[R22] 截取子串
来源：http://ljr.yj202588.top

echo "${s:0:5}"
来源：http://fym.zdqjudy.top

[R23] 字符串替换
来源：http://iaz.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lun.kuanghao11.cn

[R24] 大小写转换
来源：http://dbp.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mqs.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://mim.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eaz.shangyingyoupin.top

[R26] 命令替换
来源：http://uhb.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://ter.chenjidiqi.icu

[R27] 算术展开
来源：http://tab.redwolf501.top

echo $((1 + 2 * 3))
来源：http://ddw.aibaodan.cn

[R28] 浮点运算
来源：http://zwh.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://kpm.shuidangran.top

[R29] 定义函数
来源：http://rgz.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lmm.tianlin.xyz

[R30] 函数返回状态码
来源：http://hvh.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://gnw.tian-w.cn

[R31] 局部变量
来源：http://mwx.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://fhj.dianchejie.cn

[R32] 参数个数校验
来源：http://kyy.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ggw.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://yzs.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ahm.yongpay.top

[R34] 退出时清理
来源：http://gre.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://epw.epnwcf.com

[R35] 后台执行并等待
来源：http://fsq.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://not.zdqjudy.top

[R36] 并发执行多个任务
来源：http://lst.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xvu.tarul.cn

[R37] 把输出赋给变量
来源：http://vch.pengpengdd.cyou

files=$(ls -1)
来源：http://hfk.jinqigfzy.top

[R38] 管道串联
来源：http://lle.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://orq.havefunace.top

[R39] 重定向标准输出与错误
来源：http://fgv.fengsongda.top

cmd > out.log 2>&1
来源：http://tbi.hammf.cn

[R40] 追加写日志
来源：http://qiv.xylfe.cn

echo "log" >> out.log
来源：http://iez.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://lcv.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://kwf.mhx1999.top

[R42] 输入重定向
来源：http://uyl.jqgfzy.top

wc -l < a.txt
来源：http://puh.aibaodan.cn

[R43] 按名字查找文件
来源：http://mby.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://nyx.nanxinkj.top

[R44] 按修改时间查找
来源：http://jiq.cucudq.cn

find . -mtime -7 -type f
来源：http://ojz.zhixingplan.top

[R45] 批量删除
来源：http://uqd.yvedp.cn

find . -name "*.tmp" -delete
来源：http://qoq.fehbvm.com

[R46] 递归替换文件内容
来源：http://bia.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jac.52xcode.cn

[R47] sed 单行替换
来源：http://ozc.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://irq.andypj.xyz

[R48] awk 取指定列
来源：http://kgm.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://tiq.sufxvd.cn

[R49] awk 带条件
来源：http://rii.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lka.fktsv.cn

[R50] awk 求和
来源：http://irb.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://vzt.gzhubu.top

[R51] 排序去重取前几
来源：http://iuq.zdbjq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wbd.jianghu66.top

[R52] 统计行数
来源：http://hnh.316326.xyz

wc -l a.txt
来源：http://wzi.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://tik.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dzh.ydjk.org.cn

[R54] 比较两个文件
来源：http://rfx.shzxlz.cn

diff a.txt b.txt
来源：http://lfy.yvedp.cn

[R55] 压缩与解压
来源：http://wmb.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://trc.hfpthk.cn

[R56] 远程拷贝
来源：http://yym.aizwys.cn

scp file user@host:/path/
来源：http://kra.ybcxt.top

[R57] 远程执行命令
来源：http://mue.hnqzz.top

ssh user@host 'uptime'
来源：http://otl.uphjek.com

[R58] 下载文件
来源：http://ppi.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pco.hnxiangtu.top

[R59] 发 POST JSON
来源：http://svs.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://brk.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://vlo.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uam.jqgufenzy.top

[R61] 磁盘占用
来源：http://cip.fengsongda.top

df -h;  du -sh *
来源：http://fwf.fehbvm.com

[R62] 找最占空间的文件
来源：http://zrt.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://rha.yonumen.top

[R63] 内存与进程
来源：http://agj.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://zhp.xuanzx.com

[R64] 结束进程
来源：http://mko.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://fcs.aibaodan.cn

[R65] 查看端口占用
来源：http://kvj.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ujb.cashguo.top

[R66] 定时任务
来源：http://upk.yueranfly.top

crontab -e;  crontab -l
来源：http://wid.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://sfc.iojbl.cn

openssl rand -hex 16
来源：http://bhf.nanxinkj.top

[R68] 计算文件校验值
来源：http://goh.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://rxw.yuanzhike.top

[R69] 生成随机密码
来源：http://vsj.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://ggu.9152youxi.cn

[R70] 时间戳与互转
来源：http://rzp.hcnkem.com

date +%s;  date -d @1700000000
来源：http://wqw.aizwys.cn

[R71] 日期格式化
来源：http://ved.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://uty.hywenlv.cn

[R72] 等待端口就绪
来源：http://cyy.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://pan.zycfv.cn

[R73] 分割大日志
来源：http://vxb.bjfxy.top

split -l 1000 big.log part_
来源：http://pmb.9152youxi.cn

[R74] 批量重命名
来源：http://lwc.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nar.jqgfzy.top

[R75] 导出环境变量
来源：http://gan.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://zdu.guannengcc.top

[R76] 使用临时文件
来源：http://mnp.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kwi.jlsjyb.cn

[R77] 读取用户输入
来源：http://nzb.yj20258.top

read -rp "请输入: " ans
来源：http://pgu.wangshuangyany.cn

[R78] 交互式菜单
来源：http://jki.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://srf.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://vxt.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://meb.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://xwv.yueranfly.top

time ./run.sh
来源：http://xps.zhaomingkeji.xyz

================================================================================
来源：http://cyt.yfazqb.com


<!-- 参考信息 -->