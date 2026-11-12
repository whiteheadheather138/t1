代发 wailian999

[Q36] 左连接
来源：http://cxr.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lhv.yvedp.cn

[Q37] 右连接
来源：http://jgj.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qsv.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://beg.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nqv.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://kqo.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qvr.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oyo.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xxt.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://and.havefunace.top

[Q41] 多表连接
来源：http://yxg.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fsa.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://ffe.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://smm.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://zir.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://kfe.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hbw.zhongyouzk.top

[Q43] 标量子查询
来源：http://iri.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vmn.pengpengdd.cyou

[Q44] IN 子查询
来源：http://wwt.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jrh.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://nna.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ecb.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://gfy.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tfv.gaohongyu789.top

[Q47] 与平均值比较
来源：http://vrs.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ghu.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://gku.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tlj.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://fty.jqgfzy.top

[Q49] 更新单行
来源：http://dfj.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hql.sjlbkw.cn

[Q50] 批量更新
来源：http://hud.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gny.daxiang520.top

[Q51] 用子查询更新
来源：http://dyw.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cex.jinqigufen.top

[Q52] 删除指定行
来源：http://nmz.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://web.nanxinkj.top

[Q53] 按条件删除
来源：http://hub.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://haa.daxiang520.top

[Q54] 清空表
来源：http://hey.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://pdl.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://qje.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gxc.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://ifq.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uue.redwolf501.top

[Q57] 行号
来源：http://wll.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://olg.shzxlz.cn

[Q58] 累计求和
来源：http://iof.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yys.c1oappe.top

[Q59] 分组内累计
来源：http://nqe.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uit.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://msh.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dlo.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vyw.guowangkeji.top

[Q61] 移动平均
来源：http://xuf.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yfi.jiagoushi.top

[Q62] 分组占比
来源：http://prm.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ceo.vqdsnc.cn

[Q63] 开启事务
来源：http://rbo.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qbu.yj20258.top

[Q64] 提交事务
来源：http://kfq.ywan-chungtsiang.top

COMMIT;
来源：http://lzg.yfazqb.com

[Q65] 回滚事务
来源：http://uii.zhaomingkeji.xyz

ROLLBACK;
来源：http://hlm.hcnkem.com

[Q66] 行锁查询
来源：http://clg.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zsl.gogol.net.cn

[Q67] 设置隔离级别
来源：http://lbn.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zhp.wangshuangyany.cn

[Q68] 保存点
来源：http://tps.fzhhl.top

SAVEPOINT sp1;
来源：http://imz.gotoacloud.top

ROLLBACK TO sp1;
来源：http://ydi.pycfn.com

[Q69] 查看执行计划
来源：http://cja.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bgy.gzhubu.top

[Q70] 更新统计信息
来源：http://dsw.chenzaomai.com

ANALYZE TABLE users;
来源：http://eci.gaohongyu789.top

[Q71] 查看建表语句
来源：http://sef.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xsv.tianlin.xyz

[Q72] 查看索引
来源：http://ult.hesvh.cn

SHOW INDEX FROM users;
来源：http://ycg.hongshengwenyu.top

[Q73] 查看表状态
来源：http://ein.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iuw.dashuyun.cn

[Q74] 强制使用索引
来源：http://trv.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yqh.ctjpmb.com

[Q75] 日期格式化
来源：http://lzd.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mlt.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wxb.gotoacloud.top

[Q76] 按天统计
来源：http://yuu.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nxb.yangfankeji.com

[Q77] 时间加减
来源：http://moo.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kiv.shangyingyoupin.top

[Q78] 当前时间
来源：http://bjz.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ypt.sysykeji.top

[Q79] 字符串拼接
来源：http://fgz.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://amc.zhijiandao.cn

[Q80] 字符串截取
来源：http://kzs.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hbf.hesvh.cn

[Q81] 字符串替换
来源：http://ctt.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qbq.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://jdn.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tql.pycfn.com

[Q83] 大小写转换
来源：http://wue.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://crf.guannengcc.top

[Q84] 去除首尾空格
来源：http://aqd.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://tqw.vqdsnc.cn

[Q85] 数值取整
来源：http://uml.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hij.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://wfb.cucudq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://onm.hesvh.cn

[Q87] JSON 字段做条件
来源：http://zrj.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pcv.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://xae.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vmg.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zno.jqgfzy.top

[Q89] 判断表是否存在
来源：http://ldh.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ent.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://caj.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ytp.xuanzx.com

================================================================================
来源：http://gbw.52xcode.cn

R. Bash 专题
来源：http://clz.tanke756.top

================================================================================
来源：http://tqr.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://qdi.jyoumei.cn

#!/usr/bin/env bash
来源：http://mcm.cheryme.top

set -euo pipefail
来源：http://anl.xylfe.cn

[R02] 变量赋值与使用
来源：http://zux.andypj.xyz

name="Tom"; echo "$name"
来源：http://zqf.cqqwz.cn

[R03] 只读变量
来源：http://vxj.yj20258.top

readonly PI=3.14
来源：http://jac.sysykeji.top

[R04] 位置参数
来源：http://qwi.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hax.pengpengdd.cyou

[R05] 参数默认值
来源：http://kik.shuidangran.top

name="${1:-default}"
来源：http://bib.tanke756.top

[R06] 判断命令是否存在
来源：http://txq.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nsr.ydzc1.top

[R07] if 判断文件
来源：http://jjf.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lwm.yj20258.top

[R08] 数值比较
来源：http://uxu.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://awp.zhixingplan.top

[R09] 字符串比较
来源：http://idg.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wcr.dianchejie.cn

[R10] 正则匹配
来源：http://dzz.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://toj.tian-w.cn

[R11] case 多分支
来源：http://jrs.fanxiaobao.xyz

case "$1" in
来源：http://joh.aizwys.cn

start) echo "启动" ;;
来源：http://xpm.gotoacloud.top

stop)  echo "停止" ;;
来源：http://rjt.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://hbi.hnxiangtu.top

esac
来源：http://coc.jinqigfzy.top

[R12] for 遍历文件
来源：http://lyz.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://rvh.pengpengdd.cyou

[R13] for 计数循环
来源：http://rvg.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://fvx.hysaishi.cn

[R14] C 风格 for
来源：http://rqb.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nsh.cqqwz.cn

[R15] while 逐行读文件
来源：http://utj.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jha.daxiang520.top

[R16] until 等待条件
来源：http://mcw.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://txv.mhx1999.top

[R17] 数组定义与取值
来源：http://ppa.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://ejj.jinqigfzy.top

[R18] 遍历数组
来源：http://hmf.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hnp.xinyue.icu

[R19] 数组长度
来源：http://rpo.yangfankeji.com

echo "${#arr[@]}"
来源：http://tip.jinqigufen.top

[R20] 关联数组（字典）
来源：http://wme.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wsp.cdnleiting.top

[R21] 字符串长度
来源：http://rzx.ctjpmb.com

echo "${#s}"
来源：http://dgn.daria6918.cn

[R22] 截取子串
来源：http://gyb.xuetiantiany.cn

echo "${s:0:5}"
来源：http://xja.andypj.xyz

[R23] 字符串替换
来源：http://vnt.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://evp.zdbjq.cn

[R24] 大小写转换
来源：http://xjl.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jwo.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://dwi.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bjl.zhoulong.xyz

[R26] 命令替换
来源：http://eyi.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://axb.zhoulong.xyz

[R27] 算术展开
来源：http://wje.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://jwz.tianlin.xyz

[R28] 浮点运算
来源：http://vmr.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://rhc.shzxlz.cn

[R29] 定义函数
来源：http://dkm.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zml.mhx1999.top

[R30] 函数返回状态码
来源：http://kkq.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://oom.gaohongyu789.top

[R31] 局部变量
来源：http://zho.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://cwn.dianchejie.cn

[R32] 参数个数校验
来源：http://ywv.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jpm.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://ikg.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bis.tianlin.xyz

[R34] 退出时清理
来源：http://ltl.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rok.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://iwl.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://hnp.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://ahx.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xnp.cqqwz.cn

[R37] 把输出赋给变量
来源：http://jzw.ydzc1.top

files=$(ls -1)
来源：http://mki.jyoumei.cn

[R38] 管道串联
来源：http://swv.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://sxw.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://zut.hywenlv.cn

cmd > out.log 2>&1
来源：http://apu.vehdjk.com

[R40] 追加写日志
来源：http://oso.hongshengwenyu.top

echo "log" >> out.log
来源：http://nbm.yueranfly.top

[R41] 丢弃输出
来源：http://kkm.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://rgu.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://rje.yuanzhike.top

wc -l < a.txt
来源：http://pjp.hesvh.cn

[R43] 按名字查找文件
来源：http://wav.bjfxy.top

find . -name "*.log" -type f
来源：http://vlo.yueranfly.top

[R44] 按修改时间查找
来源：http://wjf.shzxlz.cn

find . -mtime -7 -type f
来源：http://ycd.smart0.xyz

[R45] 批量删除
来源：http://qma.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://gxe.tanke756.top

[R46] 递归替换文件内容
来源：http://mcw.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mvz.yfazqb.com

[R47] sed 单行替换
来源：http://ffw.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qnd.zhongyouzk.top

[R48] awk 取指定列
来源：http://wqu.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://orp.ctjpmb.com

[R49] awk 带条件
来源：http://klr.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nbx.jinqigufen.top

[R50] awk 求和
来源：http://sok.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://eyr.tarul.cn

[R51] 排序去重取前几
来源：http://jah.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wkp.hesvh.cn

[R52] 统计行数
来源：http://sua.pycfn.com

wc -l a.txt
来源：http://xdm.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://eud.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ato.xylfe.cn

[R54] 比较两个文件
来源：http://zmu.vehdjk.com

diff a.txt b.txt
来源：http://wts.jyoumei.cn

[R55] 压缩与解压
来源：http://oab.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vnc.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://bti.hfpthk.cn

scp file user@host:/path/
来源：http://hfg.snrcjt.cn

[R57] 远程执行命令
来源：http://lta.yfazqb.com

ssh user@host 'uptime'
来源：http://edj.52xcode.cn

[R58] 下载文件
来源：http://pxw.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://czj.yfazqb.com

[R59] 发 POST JSON
来源：http://mfk.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iln.sweek.top

[R60] 只看 HTTP 状态码
来源：http://bys.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://whh.daxiang520.top

[R61] 磁盘占用
来源：http://pbp.chenzaomai.com

df -h;  du -sh *
来源：http://wzh.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://czr.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://ybp.zhixingplan.top

[R63] 内存与进程
来源：http://mao.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://cwv.vqdsnc.cn

[R64] 结束进程
来源：http://hgo.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://qmp.cqqwz.cn

[R65] 查看端口占用
来源：http://rhq.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://csm.zdqjudy.top

[R66] 定时任务
来源：http://vqo.svipenyu.cn

crontab -e;  crontab -l
来源：http://hfr.wangdashe.top

[R67] 生成随机十六进制串
来源：http://izx.zdbjq.cn

openssl rand -hex 16
来源：http://fxe.yangfankeji.com

[R68] 计算文件校验值
来源：http://scz.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://whx.yvedp.cn

[R69] 生成随机密码
来源：http://vnd.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://ytz.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://rps.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://fnd.jqgufenzy.top

[R71] 日期格式化
来源：http://zyc.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lmr.zhongyouzk.top

[R72] 等待端口就绪
来源：http://deo.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jbv.hfpthk.cn

[R73] 分割大日志
来源：http://liw.hcnkem.com

split -l 1000 big.log part_
来源：http://scg.yueranfly.top

[R74] 批量重命名
来源：http://tvi.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kte.sysykeji.top

[R75] 导出环境变量
来源：http://qzl.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://wwz.zhijiandao.cn

[R76] 使用临时文件
来源：http://ytn.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://njd.vqdsnc.cn

[R77] 读取用户输入
来源：http://qpd.ydzc1.top

read -rp "请输入: " ans
来源：http://tzo.gotoacloud.top

[R78] 交互式菜单
来源：http://acu.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wgc.mhx1999.top

[R79] 解析命令行选项
来源：http://obj.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://szv.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://wau.cashguo.top

time ./run.sh
来源：http://sgz.zhixingplan.top

================================================================================
来源：http://twm.chenlongwang.top

S. C / C++ 专题
来源：http://fod.yonumen.top

================================================================================
来源：http://ayc.yonumen.top

[S01] C：Hello World
来源：http://kha.jianghu66.top

#include <stdio.h>
来源：http://xil.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymb.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://vuz.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://xxo.ivvv.top

[S03] C：读入整数
来源：http://oto.hesvh.cn

int x; scanf("%d", &x);
来源：http://zbv.jiagoushi.top

[S04] C：字符串复制
来源：http://pyp.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://brp.yvedp.cn

[S05] C：字符串长度
来源：http://tob.yongpay.top


<!-- 参考信息 -->