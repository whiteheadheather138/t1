代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ojg.yongpay.top

[Q28] 求和与平均
来源：http://bbb.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yxb.316326.xyz

[Q29] 最大最小值
来源：http://erx.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yjx.nanxinkj.top

[Q30] 分组统计
来源：http://ovm.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tin.yueranfly.top

[Q31] 分组后过滤
来源：http://hwx.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yfb.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://eng.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ebe.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://upg.yongpay.top

[Q33] 多列分组
来源：http://dvz.xziqi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vie.0kj1m.cn

[Q34] 每组取第一条
来源：http://aem.fzhhl.top

SELECT * FROM (
来源：http://pwf.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cjo.cqqwz.cn

) t WHERE rn = 1;
来源：http://dmj.dianchejie.cn

[Q35] 内连接
来源：http://bsk.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fin.yfazqb.com

[Q36] 左连接
来源：http://kqs.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rzs.yonumen.top

[Q37] 右连接
来源：http://fjs.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ndy.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iks.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dao.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://tbx.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ath.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dpc.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://nyu.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rlf.cheryme.top

[Q41] 多表连接
来源：http://ryi.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hed.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://gcw.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://uco.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://btq.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://bsk.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fkj.aizwys.cn

[Q43] 标量子查询
来源：http://yju.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wzi.zdbjq.cn

[Q44] IN 子查询
来源：http://uod.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qak.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://nxh.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pkp.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xvl.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zjh.snrcjt.cn

[Q47] 与平均值比较
来源：http://yxt.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cje.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://fis.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lgj.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://iec.wangdashe.top

[Q49] 更新单行
来源：http://slp.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tdu.guannengcc.top

[Q50] 批量更新
来源：http://bkc.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rcw.ctjpmb.com

[Q51] 用子查询更新
来源：http://afb.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mma.yuxming.cn

[Q52] 删除指定行
来源：http://cnk.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://uin.xziqi.cn

[Q53] 按条件删除
来源：http://gny.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rme.xylfe.cn

[Q54] 清空表
来源：http://cdt.ivvv.top

TRUNCATE TABLE logs;
来源：http://oit.guannengcc.top

[Q55] 排名（并列占位）
来源：http://bix.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rvs.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://tnk.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mee.vqdsnc.cn

[Q57] 行号
来源：http://hzb.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bjs.hesvh.cn

[Q58] 累计求和
来源：http://kjl.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dmf.shangyingyoupin.top

[Q59] 分组内累计
来源：http://udo.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gqp.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://nwl.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bri.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yhm.smart0.xyz

[Q61] 移动平均
来源：http://fgd.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lap.quarkkingdee.top

[Q62] 分组占比
来源：http://gsf.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ylz.yj20258888.top

[Q63] 开启事务
来源：http://wdm.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ozg.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://moe.ppjwa.cn

COMMIT;
来源：http://xiy.yfazqb.com

[Q65] 回滚事务
来源：http://tls.fanxiaobao.xyz

ROLLBACK;
来源：http://yqd.xuanzx.com

[Q66] 行锁查询
来源：http://ewz.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mjp.hywenlv.cn

[Q67] 设置隔离级别
来源：http://cnz.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gtt.gzhubu.top

[Q68] 保存点
来源：http://jkk.guannengcc.top

SAVEPOINT sp1;
来源：http://jdg.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://dwh.ydzc1.top

[Q69] 查看执行计划
来源：http://cfb.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kjy.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://olt.daria6918.cn

ANALYZE TABLE users;
来源：http://idz.zycfv.cn

[Q71] 查看建表语句
来源：http://ygj.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vpc.snrcjt.cn

[Q72] 查看索引
来源：http://cun.guowangkeji.top

SHOW INDEX FROM users;
来源：http://srx.fehbvm.com

[Q73] 查看表状态
来源：http://iqg.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eye.sxryk.cn

[Q74] 强制使用索引
来源：http://fkf.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://crc.cheryme.top

[Q75] 日期格式化
来源：http://yxx.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://snp.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rjj.jianghu66.top

[Q76] 按天统计
来源：http://knl.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://csr.cucudq.cn

[Q77] 时间加减
来源：http://jhg.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mae.zhengqikj.top

[Q78] 当前时间
来源：http://kst.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gvn.9152youxi.cn

[Q79] 字符串拼接
来源：http://mon.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rtj.zhijiandao.cn

[Q80] 字符串截取
来源：http://wyp.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dhl.gzhubu.top

[Q81] 字符串替换
来源：http://ikt.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wlh.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://dgd.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bgl.pycfn.com

[Q83] 大小写转换
来源：http://mda.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pmk.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://wsm.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://web.zhoulong.xyz

[Q85] 数值取整
来源：http://wqf.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://trt.hammf.cn

[Q86] 读取 JSON 字段
来源：http://awd.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://san.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://nve.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zft.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://tgu.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hvb.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uyi.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://uog.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xwd.ctjpmb.com

[Q90] 生成序号列
来源：http://mic.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fsz.cdnleiting.top

================================================================================
来源：http://lsz.fktsv.cn

R. Bash 专题
来源：http://run.pengpengdd.cyou

================================================================================
来源：http://bem.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://smq.meibo888.top

#!/usr/bin/env bash
来源：http://ljo.havefunace.top

set -euo pipefail
来源：http://eeo.yuanzhike.top

[R02] 变量赋值与使用
来源：http://hen.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://lxq.ydjk.org.cn

[R03] 只读变量
来源：http://smv.ydjk.org.cn

readonly PI=3.14
来源：http://kfq.wangdashe.top

[R04] 位置参数
来源：http://xuk.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kjb.yuanzhike.top

[R05] 参数默认值
来源：http://uxg.zdqjudy.top

name="${1:-default}"
来源：http://xvd.yueranfly.top

[R06] 判断命令是否存在
来源：http://xpa.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cfa.yangfankeji.com

[R07] if 判断文件
来源：http://exm.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ttk.aibaodan.cn

[R08] 数值比较
来源：http://woi.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jjz.hesvh.cn

[R09] 字符串比较
来源：http://rsy.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zlo.yongpay.top

[R10] 正则匹配
来源：http://bpz.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zct.hysaishi.cn

[R11] case 多分支
来源：http://ngs.cdnleiting.top

case "$1" in
来源：http://rgc.cheryme.top

start) echo "启动" ;;
来源：http://off.xziqi.cn

stop)  echo "停止" ;;
来源：http://cnw.birdmap.top

*)     echo "未知命令" ;;
来源：http://abl.ivvv.top

esac
来源：http://qcg.havefunace.top

[R12] for 遍历文件
来源：http://fty.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://ecb.nanxinkj.top

[R13] for 计数循环
来源：http://jic.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://puu.xinyue.icu

[R14] C 风格 for
来源：http://fvg.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zmt.meibo888.top

[R15] while 逐行读文件
来源：http://xhl.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://plv.yongpay.top

[R16] until 等待条件
来源：http://vyu.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zcx.ppjwa.cn

[R17] 数组定义与取值
来源：http://fqn.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://lvp.cashguo.top

[R18] 遍历数组
来源：http://vby.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jgv.tarul.cn

[R19] 数组长度
来源：http://cnv.xziqi.cn

echo "${#arr[@]}"
来源：http://yxx.jinqigufen.top

[R20] 关联数组（字典）
来源：http://vkr.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jvw.cheryme.top

[R21] 字符串长度
来源：http://goa.yj202588.top

echo "${#s}"
来源：http://mxq.shzxlz.cn

[R22] 截取子串
来源：http://ezc.hywenlv.cn

echo "${s:0:5}"
来源：http://wdo.zdbjq.cn

[R23] 字符串替换
来源：http://sbf.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hzl.xylfe.cn

[R24] 大小写转换
来源：http://rxv.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://hra.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://qdq.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bzk.meibo888.top

[R26] 命令替换
来源：http://tna.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://noe.hcnkem.com

[R27] 算术展开
来源：http://wfb.xylfe.cn

echo $((1 + 2 * 3))
来源：http://ybt.sufxvd.cn

[R28] 浮点运算
来源：http://agi.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://bbr.epnwcf.com

[R29] 定义函数
来源：http://rdp.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kym.uphjek.com

[R30] 函数返回状态码
来源：http://bcb.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://ozj.aibaodan.cn

[R31] 局部变量
来源：http://zog.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://blg.cheryme.top

[R32] 参数个数校验
来源：http://olq.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tcf.yj202588.top

[R33] 捕获错误并提示行号
来源：http://pky.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iqy.yongpay.top

[R34] 退出时清理
来源：http://idb.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://diw.zhixingplan.top

[R35] 后台执行并等待
来源：http://kfy.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://gfc.cucudq.cn

[R36] 并发执行多个任务
来源：http://gxn.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jde.hammf.cn

[R37] 把输出赋给变量
来源：http://lgo.birdmap.top

files=$(ls -1)
来源：http://ayg.yvedp.cn

[R38] 管道串联
来源：http://shc.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://ycc.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://wee.yanxiufei.cn

cmd > out.log 2>&1
来源：http://kch.xuanzx.com

[R40] 追加写日志
来源：http://sve.daria6918.cn

echo "log" >> out.log
来源：http://wzr.wangshuangyany.cn

[R41] 丢弃输出
来源：http://ytr.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://ayb.nanxinkj.top

[R42] 输入重定向
来源：http://chu.nwbrower.top

wc -l < a.txt
来源：http://tav.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://zss.jinqigfzy.top

find . -name "*.log" -type f
来源：http://tvs.ctjpmb.com

[R44] 按修改时间查找
来源：http://uih.zhijiandao.cn

find . -mtime -7 -type f
来源：http://osl.0kj1m.cn

[R45] 批量删除
来源：http://aqe.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://vod.cheryme.top

[R46] 递归替换文件内容
来源：http://uke.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hdk.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://wyy.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://chz.chenjidiqi.icu

[R48] awk 取指定列
来源：http://lwt.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://ojs.xuetiantiany.cn

[R49] awk 带条件
来源：http://fpj.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dda.svipenyu.cn

[R50] awk 求和
来源：http://nkt.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uhb.tianlin.xyz

[R51] 排序去重取前几
来源：http://uir.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://duw.jinqigufen.top

[R52] 统计行数
来源：http://xbh.cashguo.top

wc -l a.txt
来源：http://ixl.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://hir.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zku.gaohongyu789.top

[R54] 比较两个文件
来源：http://upz.ydzc1.top

diff a.txt b.txt
来源：http://sew.sweek.top

[R55] 压缩与解压
来源：http://owi.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yfw.zhoulong.xyz

[R56] 远程拷贝
来源：http://qsv.chenlongwang.top

scp file user@host:/path/
来源：http://czz.havefunace.top

[R57] 远程执行命令
来源：http://vsz.yangfankeji.com

ssh user@host 'uptime'
来源：http://nun.zhongyouzk.top

[R58] 下载文件
来源：http://vwf.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qqz.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://cgr.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qlb.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://fot.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rpu.yj20258.top

[R61] 磁盘占用
来源：http://ppa.shangyingyoupin.top

df -h;  du -sh *
来源：http://gzz.uphjek.com

[R62] 找最占空间的文件
来源：http://cgq.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://exg.shanyushiyangtech.top

[R63] 内存与进程
来源：http://ack.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://yfi.cucudq.cn

[R64] 结束进程
来源：http://kbp.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://lcm.hongshengwenyu.top

[R65] 查看端口占用
来源：http://jdh.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zen.yuanzhike.top

[R66] 定时任务
来源：http://vkt.epnwcf.com

crontab -e;  crontab -l
来源：http://jad.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://rtm.zdbjq.cn

openssl rand -hex 16
来源：http://wrb.bjfxy.top

[R68] 计算文件校验值
来源：http://vtl.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://cly.chenjidiqi.icu

[R69] 生成随机密码
来源：http://jfj.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://dwi.zycfv.cn

[R70] 时间戳与互转
来源：http://ajh.gzhubu.top

date +%s;  date -d @1700000000
来源：http://aco.smart0.xyz

[R71] 日期格式化
来源：http://emz.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rad.zhengqikj.top

[R72] 等待端口就绪
来源：http://gdg.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://oxj.pengpengdd.cyou

[R73] 分割大日志
来源：http://bcn.0kj1m.cn

split -l 1000 big.log part_
来源：http://qrx.ybcxt.top

[R74] 批量重命名
来源：http://xdp.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uec.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://ggl.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://qkn.jianghu66.top

[R76] 使用临时文件
来源：http://rrv.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ulr.feifeiyinyue.top

[R77] 读取用户输入
来源：http://pwe.yanxiufei.cn


<!-- 参考信息 -->