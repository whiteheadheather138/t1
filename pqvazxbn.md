代发 wailian999

[Q36] 左连接
来源：http://ojb.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zoi.cdnleiting.top

[Q37] 右连接
来源：http://lcu.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kdt.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iux.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dhz.tarul.cn

[Q39] 自连接（查上下级）
来源：http://onw.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hkm.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ijz.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vhk.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cjk.chenlongwang.top

[Q41] 多表连接
来源：http://pph.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://obq.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://jtx.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://dta.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://puf.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://tat.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ost.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://tsz.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://llr.ydjk.org.cn

[Q44] IN 子查询
来源：http://kam.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zbd.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://kco.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ssv.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://rpr.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kca.pycfn.com

[Q47] 与平均值比较
来源：http://dfo.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ehv.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://hha.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://akx.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://uje.fehbvm.com

[Q49] 更新单行
来源：http://cnc.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rso.shzxlz.cn

[Q50] 批量更新
来源：http://xan.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kgr.andypj.xyz

[Q51] 用子查询更新
来源：http://rms.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://paa.hfpthk.cn

[Q52] 删除指定行
来源：http://krh.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://ydz.sufxvd.cn

[Q53] 按条件删除
来源：http://nrm.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iio.fehbvm.com

[Q54] 清空表
来源：http://des.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://fpj.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://lex.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pbf.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://szj.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rgj.yj20258.top

[Q57] 行号
来源：http://ldo.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kwe.iojbl.cn

[Q58] 累计求和
来源：http://wni.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kny.wangshuangyany.cn

[Q59] 分组内累计
来源：http://nxi.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nlb.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://pfn.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vuy.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kcu.zhoulong.xyz

[Q61] 移动平均
来源：http://goe.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dma.bbcook.cn

[Q62] 分组占比
来源：http://dzb.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tjg.yangfankeji.com

[Q63] 开启事务
来源：http://tuv.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wqn.tanke756.top

[Q64] 提交事务
来源：http://oar.ybcxt.top

COMMIT;
来源：http://gxo.jyoumei.cn

[Q65] 回滚事务
来源：http://zvo.kuanghao11.cn

ROLLBACK;
来源：http://omr.gotoacloud.top

[Q66] 行锁查询
来源：http://gii.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xoy.cashguo.top

[Q67] 设置隔离级别
来源：http://yvi.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cxi.jlsjyb.cn

[Q68] 保存点
来源：http://ety.yvedp.cn

SAVEPOINT sp1;
来源：http://cup.pycfn.com

ROLLBACK TO sp1;
来源：http://mrg.meibo888.top

[Q69] 查看执行计划
来源：http://toy.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgv.fktsv.cn

[Q70] 更新统计信息
来源：http://wxn.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://ibu.hywenlv.cn

[Q71] 查看建表语句
来源：http://asj.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ete.fzhhl.top

[Q72] 查看索引
来源：http://cap.smart0.xyz

SHOW INDEX FROM users;
来源：http://vta.fehbvm.com

[Q73] 查看表状态
来源：http://sln.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qup.iojbl.cn

[Q74] 强制使用索引
来源：http://xoi.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdn.guannengcc.top

[Q75] 日期格式化
来源：http://xiy.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://imh.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yiz.daria6918.cn

[Q76] 按天统计
来源：http://pvf.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://grk.feifeiyinyue.top

[Q77] 时间加减
来源：http://umb.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dzc.pycfn.com

[Q78] 当前时间
来源：http://cyv.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sqz.shzxlz.cn

[Q79] 字符串拼接
来源：http://pld.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xyd.yuanzhike.top

[Q80] 字符串截取
来源：http://hmy.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xct.havefunace.top

[Q81] 字符串替换
来源：http://bgb.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://poc.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://zmm.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ntf.sxryk.cn

[Q83] 大小写转换
来源：http://hnj.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oom.uphjek.com

[Q84] 去除首尾空格
来源：http://sqs.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://hae.jinqigfzy.top

[Q85] 数值取整
来源：http://leg.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qkg.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://jqn.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qlz.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://tlx.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dyk.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://ytp.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ibp.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bga.xylfe.cn

[Q89] 判断表是否存在
来源：http://cha.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ybn.jinqigufen.top

[Q90] 生成序号列
来源：http://zlr.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ewz.yj20258888.top

================================================================================
来源：http://css.52xcode.cn

R. Bash 专题
来源：http://dxx.fzhhl.top

================================================================================
来源：http://xpc.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://pjw.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://wni.yangfankeji.com

set -euo pipefail
来源：http://ufq.shuidangran.top

[R02] 变量赋值与使用
来源：http://guc.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://noi.haohaochexian.top

[R03] 只读变量
来源：http://nha.bbcook.cn

readonly PI=3.14
来源：http://yei.pengpengdd.cyou

[R04] 位置参数
来源：http://kex.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iwc.svipenyu.cn

[R05] 参数默认值
来源：http://ufy.ybcxt.top

name="${1:-default}"
来源：http://eye.9152youxi.cn

[R06] 判断命令是否存在
来源：http://sxy.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nut.fehbvm.com

[R07] if 判断文件
来源：http://irh.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sqz.9152youxi.cn

[R08] 数值比较
来源：http://goj.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fdq.shangyingyoupin.top

[R09] 字符串比较
来源：http://vws.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fyn.hammf.cn

[R10] 正则匹配
来源：http://wdt.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rmz.shangyingyoupin.top

[R11] case 多分支
来源：http://xbv.snrcjt.cn

case "$1" in
来源：http://txu.hywenlv.cn

start) echo "启动" ;;
来源：http://ivb.vehdjk.com

stop)  echo "停止" ;;
来源：http://uey.tarul.cn

*)     echo "未知命令" ;;
来源：http://get.xuetiantiany.cn

esac
来源：http://hdv.hywenlv.cn

[R12] for 遍历文件
来源：http://cad.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://zfy.wangshuangyany.cn

[R13] for 计数循环
来源：http://bmm.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://ruq.yj20258888.top

[R14] C 风格 for
来源：http://ucz.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gkr.zdqjudy.top

[R15] while 逐行读文件
来源：http://xym.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fac.jlsjyb.cn

[R16] until 等待条件
来源：http://rsb.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://khh.jqgufenzy.top

[R17] 数组定义与取值
来源：http://thb.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://vxk.hnqzz.top

[R18] 遍历数组
来源：http://zyw.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dmf.zhengqikj.top

[R19] 数组长度
来源：http://nze.cqqwz.cn

echo "${#arr[@]}"
来源：http://wod.aibaodan.cn

[R20] 关联数组（字典）
来源：http://vfe.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ein.meibo888.top

[R21] 字符串长度
来源：http://cin.gzhubu.top

echo "${#s}"
来源：http://wxc.wangshuangyany.cn

[R22] 截取子串
来源：http://wtt.nanxuanxn.top

echo "${s:0:5}"
来源：http://nah.ctjpmb.com

[R23] 字符串替换
来源：http://kte.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zcg.zhengqikj.top

[R24] 大小写转换
来源：http://xgv.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zwp.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://nir.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqn.zdbjq.cn

[R26] 命令替换
来源：http://dma.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://akv.aizwys.cn

[R27] 算术展开
来源：http://evp.sweek.top

echo $((1 + 2 * 3))
来源：http://xze.9152youxi.cn

[R28] 浮点运算
来源：http://gir.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://jea.52xcode.cn

[R29] 定义函数
来源：http://kqh.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nzc.andypj.xyz

[R30] 函数返回状态码
来源：http://muv.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://tst.cdnleiting.top

[R31] 局部变量
来源：http://avc.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://zey.yvedp.cn

[R32] 参数个数校验
来源：http://cac.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cvt.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://eac.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fsx.yj202588.top

[R34] 退出时清理
来源：http://zqf.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://ubb.cheryme.top

[R35] 后台执行并等待
来源：http://mox.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sey.xinyue.icu

[R36] 并发执行多个任务
来源：http://zjq.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfp.zdbjq.cn

[R37] 把输出赋给变量
来源：http://lea.hnqzz.top

files=$(ls -1)
来源：http://wvq.wangdashe.top

[R38] 管道串联
来源：http://zsh.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://sxi.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://gnb.bbcook.cn

cmd > out.log 2>&1
来源：http://ucj.pengpengdd.cyou

[R40] 追加写日志
来源：http://wdn.kuanghao11.cn

echo "log" >> out.log
来源：http://yys.wangshuangyany.cn

[R41] 丢弃输出
来源：http://zfd.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://ahn.fzhhl.top

[R42] 输入重定向
来源：http://pgj.tianlin.xyz

wc -l < a.txt
来源：http://nqy.nanxinkj.top

[R43] 按名字查找文件
来源：http://zih.ydzc1.top

find . -name "*.log" -type f
来源：http://zhu.quarkkingdee.top

[R44] 按修改时间查找
来源：http://aqq.yj202588.top

find . -mtime -7 -type f
来源：http://aop.xinyue.icu

[R45] 批量删除
来源：http://xrd.guannengcc.top

find . -name "*.tmp" -delete
来源：http://lof.gotoacloud.top

[R46] 递归替换文件内容
来源：http://fyp.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yfk.yueranfly.top

[R47] sed 单行替换
来源：http://thr.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zpo.pengpengdd.cyou

[R48] awk 取指定列
来源：http://qak.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://oyc.yanxiufei.cn

[R49] awk 带条件
来源：http://abj.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://msx.ctjpmb.com

[R50] awk 求和
来源：http://lxo.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://jvn.aibaodan.cn

[R51] 排序去重取前几
来源：http://hcg.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://aqh.uphjek.com

[R52] 统计行数
来源：http://gvv.hcnkem.com

wc -l a.txt
来源：http://rzb.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://dod.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nne.c1oappe.top

[R54] 比较两个文件
来源：http://kkm.zhiwuduotai.top

diff a.txt b.txt
来源：http://ucb.zhixingplan.top

[R55] 压缩与解压
来源：http://ngy.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zrb.jqgufenzy.top

[R56] 远程拷贝
来源：http://lqg.uphjek.com

scp file user@host:/path/
来源：http://bbk.hammf.cn

[R57] 远程执行命令
来源：http://hma.quarkkingdee.top

ssh user@host 'uptime'
来源：http://cfd.yfazqb.com

[R58] 下载文件
来源：http://awc.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hfr.yj20258.top

[R59] 发 POST JSON
来源：http://asd.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tgb.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://cbg.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mvj.shangyingyoupin.top

[R61] 磁盘占用
来源：http://qgm.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://guv.zdqjudy.top

[R62] 找最占空间的文件
来源：http://thc.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://rrn.yueranfly.top

[R63] 内存与进程
来源：http://rtr.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://bsx.kuanghao11.cn

[R64] 结束进程
来源：http://zqy.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://lhv.zdqjudy.top

[R65] 查看端口占用
来源：http://tjh.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oqd.hysaishi.cn

[R66] 定时任务
来源：http://oxd.wangdashe.top

crontab -e;  crontab -l
来源：http://kgc.yonumen.top

[R67] 生成随机十六进制串
来源：http://cfr.jlsjyb.cn

openssl rand -hex 16
来源：http://ujz.guannengcc.top

[R68] 计算文件校验值
来源：http://zrt.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://two.yvedp.cn

[R69] 生成随机密码
来源：http://daq.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://bdo.zhixingplan.top

[R70] 时间戳与互转
来源：http://qlz.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://smo.nwbrower.top

[R71] 日期格式化
来源：http://ihm.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://urb.tanke756.top

[R72] 等待端口就绪
来源：http://ybj.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://giy.xziqi.cn

[R73] 分割大日志
来源：http://jzn.haohaochexian.top

split -l 1000 big.log part_
来源：http://cwa.pycfn.com

[R74] 批量重命名
来源：http://tgx.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yws.pengpengdd.cyou

[R75] 导出环境变量
来源：http://mve.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://tfp.xylfe.cn

[R76] 使用临时文件
来源：http://xvk.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vux.jyoumei.cn

[R77] 读取用户输入
来源：http://ugm.c1oappe.top

read -rp "请输入: " ans
来源：http://pbt.snrcjt.cn

[R78] 交互式菜单
来源：http://kry.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://opg.vehdjk.com

[R79] 解析命令行选项
来源：http://roq.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lly.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://xqm.pengpengdd.cyou

time ./run.sh
来源：http://jps.cdnleiting.top

================================================================================
来源：http://lnc.tanke756.top

S. C / C++ 专题
来源：http://apv.zhengqikj.top

================================================================================
来源：http://lti.c1oappe.top

[S01] C：Hello World
来源：http://sdx.0kj1m.cn

#include <stdio.h>
来源：http://zio.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pcm.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://nqk.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://erw.dianchejie.cn

[S03] C：读入整数
来源：http://uzf.havefunace.top

int x; scanf("%d", &x);
来源：http://jcy.xuetiantiany.cn

[S04] C：字符串复制
来源：http://ijf.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://utn.aibaodan.cn

[S05] C：字符串长度
来源：http://ysi.hysaishi.cn


<!-- 参考信息 -->