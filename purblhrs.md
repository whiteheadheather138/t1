代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xvc.dianchejie.cn

) t WHERE rn = 1;
来源：http://oir.daria6918.cn

[Q35] 内连接
来源：http://phb.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gde.zhiwuduotai.top

[Q36] 左连接
来源：http://tij.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bqk.gogol.net.cn

[Q37] 右连接
来源：http://dgs.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yrh.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://bhv.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://thb.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://ejw.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dob.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pay.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oir.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fua.jiagoushi.top

[Q41] 多表连接
来源：http://irt.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jpo.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://vqw.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://xug.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://biu.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://iuj.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://boe.zhixingplan.top

[Q43] 标量子查询
来源：http://oqw.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://peb.jinqigufen.top

[Q44] IN 子查询
来源：http://uxt.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ptg.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://guk.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kss.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qjw.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hvr.cheryme.top

[Q47] 与平均值比较
来源：http://brn.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ouy.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://qzy.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wlt.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://gfc.vqdsnc.cn

[Q49] 更新单行
来源：http://vxa.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://alo.jqgfzy.top

[Q50] 批量更新
来源：http://tiz.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qtp.nwbrower.top

[Q51] 用子查询更新
来源：http://uyj.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rzx.xinyue.icu

[Q52] 删除指定行
来源：http://bwf.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://zcc.guowangkeji.top

[Q53] 按条件删除
来源：http://sol.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zde.fehbvm.com

[Q54] 清空表
来源：http://nea.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://cfe.yvedp.cn

[Q55] 排名（并列占位）
来源：http://zdx.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://awd.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://cbl.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pad.jyoumei.cn

[Q57] 行号
来源：http://nof.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://trp.aibaodan.cn

[Q58] 累计求和
来源：http://qyr.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lej.pycfn.com

[Q59] 分组内累计
来源：http://ain.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tbb.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://tfm.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kdz.yongpay.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hgw.fktsv.cn

[Q61] 移动平均
来源：http://ezd.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uqh.shanyushiyangtech.top

[Q62] 分组占比
来源：http://kho.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jqh.yongpay.top

[Q63] 开启事务
来源：http://qir.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://viu.aizwys.cn

[Q64] 提交事务
来源：http://liq.shanyushiyangkeji.top

COMMIT;
来源：http://ofe.sysykeji.top

[Q65] 回滚事务
来源：http://wlb.cucudq.cn

ROLLBACK;
来源：http://gvq.yj202588.top

[Q66] 行锁查询
来源：http://fxj.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nmr.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://ldr.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aty.aibaodan.cn

[Q68] 保存点
来源：http://kln.guowangkeji.top

SAVEPOINT sp1;
来源：http://qkx.ybcxt.top

ROLLBACK TO sp1;
来源：http://rga.ivvv.top

[Q69] 查看执行计划
来源：http://vlv.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gpe.yj20258888.top

[Q70] 更新统计信息
来源：http://tus.chenzaomai.com

ANALYZE TABLE users;
来源：http://jdq.redwolf501.top

[Q71] 查看建表语句
来源：http://yiv.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://awm.nwbrower.top

[Q72] 查看索引
来源：http://guk.yueranfly.top

SHOW INDEX FROM users;
来源：http://odj.jyoumei.cn

[Q73] 查看表状态
来源：http://ioc.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://lyo.yanxiufei.cn

[Q74] 强制使用索引
来源：http://tta.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nmx.andypj.xyz

[Q75] 日期格式化
来源：http://tzl.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mmo.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ipc.gogol.net.cn

[Q76] 按天统计
来源：http://opn.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uvl.daria6918.cn

[Q77] 时间加减
来源：http://uld.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xyk.chenzaomai.com

[Q78] 当前时间
来源：http://mpg.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ovi.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://euz.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ugy.zhijiandao.cn

[Q80] 字符串截取
来源：http://zdc.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zni.dashuyun.cn

[Q81] 字符串替换
来源：http://okq.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rgl.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://qwv.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pyu.jinqigufen.top

[Q83] 大小写转换
来源：http://niv.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ckp.zhixingplan.top

[Q84] 去除首尾空格
来源：http://tvk.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://gyn.hammf.cn

[Q85] 数值取整
来源：http://gjh.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yve.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://zeb.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mvl.fengsongda.top

[Q87] JSON 字段做条件
来源：http://gjl.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ias.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://zfo.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ldy.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jlx.cashguo.top

[Q89] 判断表是否存在
来源：http://dhu.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ioe.yj202588.top

[Q90] 生成序号列
来源：http://gzd.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ohl.andypj.xyz

================================================================================
来源：http://lft.ctjpmb.com

R. Bash 专题
来源：http://otr.hcnkem.com

================================================================================
来源：http://xpm.ppjwa.cn

[R01] shebang 与严格模式
来源：http://eic.jqgfzy.top

#!/usr/bin/env bash
来源：http://zxz.chenlongwang.top

set -euo pipefail
来源：http://hta.meibo888.top

[R02] 变量赋值与使用
来源：http://psq.cqqwz.cn

name="Tom"; echo "$name"
来源：http://hbw.shuidangran.top

[R03] 只读变量
来源：http://lrx.smart0.xyz

readonly PI=3.14
来源：http://ceg.wangshuangyany.cn

[R04] 位置参数
来源：http://uuu.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oxi.svipenyu.cn

[R05] 参数默认值
来源：http://aoq.cheryme.top

name="${1:-default}"
来源：http://qfm.yvedp.cn

[R06] 判断命令是否存在
来源：http://lue.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mrc.hesvh.cn

[R07] if 判断文件
来源：http://qka.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ikl.wangdashe.top

[R08] 数值比较
来源：http://wnf.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://crb.andypj.xyz

[R09] 字符串比较
来源：http://qqt.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uap.hesvh.cn

[R10] 正则匹配
来源：http://fnm.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cjk.zhijiandao.cn

[R11] case 多分支
来源：http://ctz.hywenlv.cn

case "$1" in
来源：http://bjf.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://lzi.iojbl.cn

stop)  echo "停止" ;;
来源：http://hxe.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://ljp.tianlin.xyz

esac
来源：http://ngf.andypj.xyz

[R12] for 遍历文件
来源：http://uvs.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://zro.zdqjudy.top

[R13] for 计数循环
来源：http://uzf.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://xxr.bjfxy.top

[R14] C 风格 for
来源：http://fkc.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uby.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://bav.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hbu.yueranfly.top

[R16] until 等待条件
来源：http://ttk.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iwj.yanxiufei.cn

[R17] 数组定义与取值
来源：http://yub.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://nle.havefunace.top

[R18] 遍历数组
来源：http://wzt.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hww.gaohongyu789.top

[R19] 数组长度
来源：http://syx.nanxuanxn.top

echo "${#arr[@]}"
来源：http://dsf.ppjwa.cn

[R20] 关联数组（字典）
来源：http://ceu.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://noz.tarul.cn

[R21] 字符串长度
来源：http://jju.hcnkem.com

echo "${#s}"
来源：http://ehq.vqdsnc.cn

[R22] 截取子串
来源：http://uso.fengsongda.top

echo "${s:0:5}"
来源：http://neo.andypj.xyz

[R23] 字符串替换
来源：http://mwp.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fef.aibaodan.cn

[R24] 大小写转换
来源：http://moc.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://edj.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://knw.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://enj.tianlin.xyz

[R26] 命令替换
来源：http://pyq.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://edt.jinqigufen.top

[R27] 算术展开
来源：http://oqk.tanke756.top

echo $((1 + 2 * 3))
来源：http://loh.zhengqikj.top

[R28] 浮点运算
来源：http://vmx.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://tqr.shzxlz.cn

[R29] 定义函数
来源：http://fxf.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jhh.dashuyun.cn

[R30] 函数返回状态码
来源：http://yce.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://rzs.xuetiantiany.cn

[R31] 局部变量
来源：http://ipj.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://fdj.daxiang520.top

[R32] 参数个数校验
来源：http://pha.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nnl.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://lrm.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qcr.wangshuangyany.cn

[R34] 退出时清理
来源：http://xes.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://buy.yj20258888.top

[R35] 后台执行并等待
来源：http://emb.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pjl.hesvh.cn

[R36] 并发执行多个任务
来源：http://crh.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ubj.vehdjk.com

[R37] 把输出赋给变量
来源：http://etm.fzhhl.top

files=$(ls -1)
来源：http://kcc.shangyingyoupin.top

[R38] 管道串联
来源：http://ixo.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://ppl.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://xvd.havefunace.top

cmd > out.log 2>&1
来源：http://nth.fanxiaobao.xyz

[R40] 追加写日志
来源：http://ajy.fehbvm.com

echo "log" >> out.log
来源：http://mca.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://nxj.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://voz.jinghuilouyu.cn

[R42] 输入重定向
来源：http://ato.cqqwz.cn

wc -l < a.txt
来源：http://mov.chenzaomai.com

[R43] 按名字查找文件
来源：http://roi.andypj.xyz

find . -name "*.log" -type f
来源：http://dcw.gzhubu.top

[R44] 按修改时间查找
来源：http://nzk.havefunace.top

find . -mtime -7 -type f
来源：http://prq.fengsongda.top

[R45] 批量删除
来源：http://odp.tian-w.cn

find . -name "*.tmp" -delete
来源：http://qjm.gzhubu.top

[R46] 递归替换文件内容
来源：http://yuw.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jiq.hammf.cn

[R47] sed 单行替换
来源：http://fcg.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bvn.chenzaomai.com

[R48] awk 取指定列
来源：http://srr.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://sjr.gzhubu.top

[R49] awk 带条件
来源：http://ddb.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gmk.wangdashe.top

[R50] awk 求和
来源：http://zlt.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://sbd.guannengcc.top

[R51] 排序去重取前几
来源：http://crr.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tlx.yanxiufei.cn

[R52] 统计行数
来源：http://xfs.jqgufenzy.top

wc -l a.txt
来源：http://iyx.sweek.top

[R53] 查看文件头与实时尾
来源：http://afw.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qan.jqgufenzy.top

[R54] 比较两个文件
来源：http://ryq.nanxinkj.top

diff a.txt b.txt
来源：http://lre.sxryk.cn

[R55] 压缩与解压
来源：http://kwz.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://odi.cqqwz.cn

[R56] 远程拷贝
来源：http://jlc.dianchejie.cn

scp file user@host:/path/
来源：http://jkf.xziqi.cn

[R57] 远程执行命令
来源：http://cin.guannengcc.top

ssh user@host 'uptime'
来源：http://iuh.yvedp.cn

[R58] 下载文件
来源：http://evl.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ciq.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://ycd.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vsh.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://yfz.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xhs.ybcxt.top

[R61] 磁盘占用
来源：http://cpi.cqqwz.cn

df -h;  du -sh *
来源：http://ubs.chenzaomai.com

[R62] 找最占空间的文件
来源：http://rjt.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://djh.ivvv.top

[R63] 内存与进程
来源：http://dlb.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://nwj.epnwcf.com

[R64] 结束进程
来源：http://brj.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://odu.jinqigufen.top

[R65] 查看端口占用
来源：http://ppn.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://usw.jyoumei.cn

[R66] 定时任务
来源：http://tel.havefunace.top

crontab -e;  crontab -l
来源：http://ssq.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://jry.quarkkingdee.top

openssl rand -hex 16
来源：http://wyq.ydjk.org.cn

[R68] 计算文件校验值
来源：http://mzn.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://rba.zhongyouzk.top

[R69] 生成随机密码
来源：http://bol.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://eym.xziqi.cn

[R70] 时间戳与互转
来源：http://gfc.pycfn.com

date +%s;  date -d @1700000000
来源：http://hxn.aizwys.cn

[R71] 日期格式化
来源：http://ovd.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://btt.smart0.xyz

[R72] 等待端口就绪
来源：http://kyd.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lav.hnxiangtu.top

[R73] 分割大日志
来源：http://uhk.quarkkingdee.top

split -l 1000 big.log part_
来源：http://cvi.tarul.cn

[R74] 批量重命名
来源：http://bjl.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jnh.ydjk.org.cn

[R75] 导出环境变量
来源：http://owq.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://oxh.nwbrower.top

[R76] 使用临时文件
来源：http://pdy.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://idf.ctjpmb.com

[R77] 读取用户输入
来源：http://vrd.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://ivw.xuanzx.com

[R78] 交互式菜单
来源：http://ocv.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iqa.shuidangran.top

[R79] 解析命令行选项
来源：http://kpq.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wrg.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://rpi.shanyushiyangtech.top

time ./run.sh
来源：http://gni.ctjpmb.com

================================================================================
来源：http://onk.jianghu66.top

S. C / C++ 专题
来源：http://wdm.gaohongyu789.top

================================================================================
来源：http://yto.yuanzhike.top

[S01] C：Hello World
来源：http://foc.andypj.xyz

#include <stdio.h>
来源：http://yev.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://moo.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://lom.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://dos.316326.xyz

[S03] C：读入整数
来源：http://cvb.fzhhl.top


<!-- 参考信息 -->