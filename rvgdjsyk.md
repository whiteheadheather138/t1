代发 wailian999

[Q33] 多列分组
来源：http://mzu.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aro.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://eqt.yuanzhike.top

SELECT * FROM (
来源：http://zmd.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nkp.snrcjt.cn

) t WHERE rn = 1;
来源：http://bry.havefunace.top

[Q35] 内连接
来源：http://uvv.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pha.smart0.xyz

[Q36] 左连接
来源：http://vik.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ifi.meibo888.top

[Q37] 右连接
来源：http://zsl.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lti.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://nzz.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rsl.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://hnn.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qzt.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yta.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vdl.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cir.yueranfly.top

[Q41] 多表连接
来源：http://gzq.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gmz.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://vua.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://qhg.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://ajb.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://rxb.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://atz.sufxvd.cn

[Q43] 标量子查询
来源：http://yoj.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://otk.52xcode.cn

[Q44] IN 子查询
来源：http://ixi.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sfv.sweek.top

[Q45] EXISTS 判断存在
来源：http://cal.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hro.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hpm.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhk.kuanghao11.cn

[Q47] 与平均值比较
来源：http://xhb.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kic.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://bwv.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kwp.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://vfk.epnwcf.com

[Q49] 更新单行
来源：http://uvo.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lql.nanxuanxn.top

[Q50] 批量更新
来源：http://pep.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rse.316326.xyz

[Q51] 用子查询更新
来源：http://lnl.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kdx.sjlbkw.cn

[Q52] 删除指定行
来源：http://wjz.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://jnj.hysaishi.cn

[Q53] 按条件删除
来源：http://nzx.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lhx.andypj.xyz

[Q54] 清空表
来源：http://uqz.yongpay.top

TRUNCATE TABLE logs;
来源：http://rtp.xinyue.icu

[Q55] 排名（并列占位）
来源：http://jmm.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lcl.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://rrn.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lhz.cqqwz.cn

[Q57] 行号
来源：http://jdo.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kww.pycfn.com

[Q58] 累计求和
来源：http://snu.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fac.zycfv.cn

[Q59] 分组内累计
来源：http://dej.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ozm.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://qpr.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ryw.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vgc.9152youxi.cn

[Q61] 移动平均
来源：http://fqj.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eas.andypj.xyz

[Q62] 分组占比
来源：http://xkh.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yvt.chenzaomai.com

[Q63] 开启事务
来源：http://iri.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bpr.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://too.zhiwuduotai.top

COMMIT;
来源：http://rdp.sjlbkw.cn

[Q65] 回滚事务
来源：http://dns.epnwcf.com

ROLLBACK;
来源：http://zpp.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://bar.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gdl.tianlin.xyz

[Q67] 设置隔离级别
来源：http://fyj.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jnq.hongshengwenyu.top

[Q68] 保存点
来源：http://nha.iojbl.cn

SAVEPOINT sp1;
来源：http://req.shuidangran.top

ROLLBACK TO sp1;
来源：http://krn.jinqigfzy.top

[Q69] 查看执行计划
来源：http://xxy.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rzz.yfazqb.com

[Q70] 更新统计信息
来源：http://eru.zhixingplan.top

ANALYZE TABLE users;
来源：http://dxt.zhixingplan.top

[Q71] 查看建表语句
来源：http://hwk.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cfw.xinyue.icu

[Q72] 查看索引
来源：http://mth.zhengqikj.top

SHOW INDEX FROM users;
来源：http://jiq.hongshengwenyu.top

[Q73] 查看表状态
来源：http://zyt.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xwn.cashguo.top

[Q74] 强制使用索引
来源：http://vkq.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dhz.ybcxt.top

[Q75] 日期格式化
来源：http://bwu.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://emw.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hom.ctjpmb.com

[Q76] 按天统计
来源：http://wei.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sjc.vqdsnc.cn

[Q77] 时间加减
来源：http://usi.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://quj.gogol.net.cn

[Q78] 当前时间
来源：http://lrp.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yij.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://okb.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fop.andypj.xyz

[Q80] 字符串截取
来源：http://dzq.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zgu.gaohongyu789.top

[Q81] 字符串替换
来源：http://qoc.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bfo.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://ktm.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://asw.gotoacloud.top

[Q83] 大小写转换
来源：http://ifc.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uav.shzxlz.cn

[Q84] 去除首尾空格
来源：http://zdk.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://egd.cheryme.top

[Q85] 数值取整
来源：http://smx.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cfj.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://uye.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iyz.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://dba.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://frc.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://tbf.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ttk.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cjo.guowangkeji.top

[Q89] 判断表是否存在
来源：http://ppl.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kdi.zycfv.cn

[Q90] 生成序号列
来源：http://bqr.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mzv.aizwys.cn

================================================================================
来源：http://yku.sxryk.cn

R. Bash 专题
来源：http://nyj.iojbl.cn

================================================================================
来源：http://agq.yongpay.top

[R01] shebang 与严格模式
来源：http://doi.ppjwa.cn

#!/usr/bin/env bash
来源：http://xoi.cucudq.cn

set -euo pipefail
来源：http://fww.fzhhl.top

[R02] 变量赋值与使用
来源：http://cut.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://vwc.ppjwa.cn

[R03] 只读变量
来源：http://rvo.yuanzhike.top

readonly PI=3.14
来源：http://tgk.gogol.net.cn

[R04] 位置参数
来源：http://qzg.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jfg.sweek.top

[R05] 参数默认值
来源：http://pgi.uphjek.com

name="${1:-default}"
来源：http://yur.cdnleiting.top

[R06] 判断命令是否存在
来源：http://pnm.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://brk.gzhubu.top

[R07] if 判断文件
来源：http://ztl.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bmm.hysaishi.cn

[R08] 数值比较
来源：http://gcb.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jsk.jqgufenzy.top

[R09] 字符串比较
来源：http://skq.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mzl.hesvh.cn

[R10] 正则匹配
来源：http://mjt.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ybr.hywenlv.cn

[R11] case 多分支
来源：http://kzq.yuanzhike.top

case "$1" in
来源：http://jyy.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://kui.hywenlv.cn

stop)  echo "停止" ;;
来源：http://ixu.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://coh.xinyue.icu

esac
来源：http://gqv.birdmap.top

[R12] for 遍历文件
来源：http://lhq.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://tpu.0kj1m.cn

[R13] for 计数循环
来源：http://fgo.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://dbb.tarul.cn

[R14] C 风格 for
来源：http://uei.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mvf.redwolf501.top

[R15] while 逐行读文件
来源：http://qls.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://riq.wangshuangyany.cn

[R16] until 等待条件
来源：http://qfw.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wqp.sjlbkw.cn

[R17] 数组定义与取值
来源：http://zat.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://tnw.tanke756.top

[R18] 遍历数组
来源：http://emk.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jir.ehwqpu.com

[R19] 数组长度
来源：http://fhf.gaohongyu789.top

echo "${#arr[@]}"
来源：http://xre.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://iqh.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://adi.guowangkeji.top

[R21] 字符串长度
来源：http://xux.wangshuangyany.cn

echo "${#s}"
来源：http://lno.shangyingyoupin.top

[R22] 截取子串
来源：http://ptr.xziqi.cn

echo "${s:0:5}"
来源：http://ccv.ctjpmb.com

[R23] 字符串替换
来源：http://xar.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wwe.yangfankeji.com

[R24] 大小写转换
来源：http://cou.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ivy.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://khd.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://fdm.aizwys.cn

[R26] 命令替换
来源：http://osx.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://ryc.zdbjq.cn

[R27] 算术展开
来源：http://mnm.hnqzz.top

echo $((1 + 2 * 3))
来源：http://dok.vehdjk.com

[R28] 浮点运算
来源：http://uqd.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://wdr.yj202588.top

[R29] 定义函数
来源：http://xnr.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pip.aizwys.cn

[R30] 函数返回状态码
来源：http://gyv.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://kcb.xinyue.icu

[R31] 局部变量
来源：http://qsa.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://eni.0kj1m.cn

[R32] 参数个数校验
来源：http://fxr.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ynt.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://qbk.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hhw.fktsv.cn

[R34] 退出时清理
来源：http://tbi.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://sja.vehdjk.com

[R35] 后台执行并等待
来源：http://cec.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yut.meibo888.top

[R36] 并发执行多个任务
来源：http://ypa.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vxd.ybcxt.top

[R37] 把输出赋给变量
来源：http://mjd.hysaishi.cn

files=$(ls -1)
来源：http://jnh.sxryk.cn

[R38] 管道串联
来源：http://apz.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://cjr.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://aqy.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://xih.52xcode.cn

[R40] 追加写日志
来源：http://ypt.tianlin.xyz

echo "log" >> out.log
来源：http://cxu.svipenyu.cn

[R41] 丢弃输出
来源：http://tsf.yongpay.top

cmd >/dev/null 2>&1
来源：http://ydn.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://ftm.sxryk.cn

wc -l < a.txt
来源：http://fyf.hfpthk.cn

[R43] 按名字查找文件
来源：http://xpb.cdnleiting.top

find . -name "*.log" -type f
来源：http://kpn.xinyue.icu

[R44] 按修改时间查找
来源：http://stm.aizwys.cn

find . -mtime -7 -type f
来源：http://htn.yfazqb.com

[R45] 批量删除
来源：http://opn.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://qlw.yfazqb.com

[R46] 递归替换文件内容
来源：http://dwl.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mls.guowangkeji.top

[R47] sed 单行替换
来源：http://dgr.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://dly.nanxuanxn.top

[R48] awk 取指定列
来源：http://tiv.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://wes.0kj1m.cn

[R49] awk 带条件
来源：http://wbu.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gnh.jinqigufen.top

[R50] awk 求和
来源：http://bei.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mzx.snrcjt.cn

[R51] 排序去重取前几
来源：http://dhx.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://znq.hnxiangtu.top

[R52] 统计行数
来源：http://bor.kuanghao11.cn

wc -l a.txt
来源：http://dol.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://smp.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://izl.uphjek.com

[R54] 比较两个文件
来源：http://pvo.ivvv.top

diff a.txt b.txt
来源：http://uqi.sxryk.cn

[R55] 压缩与解压
来源：http://jlc.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://afa.yanxiufei.cn

[R56] 远程拷贝
来源：http://cei.sjlbkw.cn

scp file user@host:/path/
来源：http://mnc.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://whl.yj20258.top

ssh user@host 'uptime'
来源：http://osv.pycfn.com

[R58] 下载文件
来源：http://kel.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nwr.ctjpmb.com

[R59] 发 POST JSON
来源：http://mdi.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cei.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://mvv.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ean.fehbvm.com

[R61] 磁盘占用
来源：http://kfm.epnwcf.com

df -h;  du -sh *
来源：http://luu.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://wqt.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://jzz.chenzaomai.com

[R63] 内存与进程
来源：http://mjm.ivvv.top

free -h;  ps aux | grep nginx
来源：http://rvk.gaohongyu789.top

[R64] 结束进程
来源：http://apc.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://abt.zhijiandao.cn

[R65] 查看端口占用
来源：http://xyw.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gmg.cucudq.cn

[R66] 定时任务
来源：http://iqt.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://dvj.yvedp.cn

[R67] 生成随机十六进制串
来源：http://lah.hywenlv.cn

openssl rand -hex 16
来源：http://epn.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://vir.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wah.gogol.net.cn

[R69] 生成随机密码
来源：http://tab.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://emh.gzhubu.top

[R70] 时间戳与互转
来源：http://tbd.fktsv.cn

date +%s;  date -d @1700000000
来源：http://phi.ydzc1.top

[R71] 日期格式化
来源：http://znd.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nve.hcnkem.com

[R72] 等待端口就绪
来源：http://mqj.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qou.ydzc1.top

[R73] 分割大日志
来源：http://uxx.yj20258.top

split -l 1000 big.log part_
来源：http://vkq.jlsjyb.cn

[R74] 批量重命名
来源：http://hnf.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oab.ehwqpu.com

[R75] 导出环境变量
来源：http://ull.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://ccu.quarkkingdee.top

[R76] 使用临时文件
来源：http://xja.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mfl.shangyingyoupin.top

[R77] 读取用户输入
来源：http://lcf.316326.xyz

read -rp "请输入: " ans
来源：http://gbu.yj20258888.top

[R78] 交互式菜单
来源：http://cjr.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gom.316326.xyz

[R79] 解析命令行选项
来源：http://dyx.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zfg.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://jph.mhx1999.top

time ./run.sh
来源：http://wwq.52xcode.cn

================================================================================
来源：http://qml.svipenyu.cn

S. C / C++ 专题
来源：http://hfq.cashguo.top

================================================================================
来源：http://nxt.jianghu66.top

[S01] C：Hello World
来源：http://kkd.hongshengwenyu.top

#include <stdio.h>
来源：http://fyc.hysaishi.cn


<!-- 参考信息 -->