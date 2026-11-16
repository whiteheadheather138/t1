代发 wailian999

[Q36] 左连接
来源：http://bzu.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://thi.vqdsnc.cn

[Q37] 右连接
来源：http://oxf.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://grr.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jer.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ldy.yj20258.top

[Q39] 自连接（查上下级）
来源：http://joh.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://juj.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fqj.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yle.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uzz.52xcode.cn

[Q41] 多表连接
来源：http://fbr.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dae.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://vko.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://iwa.ivvv.top

[Q42] 连接条件附加过滤
来源：http://wfh.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://hga.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hii.chenzaomai.com

[Q43] 标量子查询
来源：http://zaq.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fka.meibo888.top

[Q44] IN 子查询
来源：http://rbt.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rht.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://tzk.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvs.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://lzo.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xnj.cashguo.top

[Q47] 与平均值比较
来源：http://hfw.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://byn.ivvv.top

[Q48] CTE 公用表表达式
来源：http://qfh.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lzu.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hes.snrcjt.cn

[Q49] 更新单行
来源：http://fbc.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qrx.yj20258.top

[Q50] 批量更新
来源：http://jpj.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfk.zhongyouzk.top

[Q51] 用子查询更新
来源：http://fnh.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eso.kuanghao11.cn

[Q52] 删除指定行
来源：http://vsu.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://isu.zycfv.cn

[Q53] 按条件删除
来源：http://kyn.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uns.guannengcc.top

[Q54] 清空表
来源：http://zxq.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://fgf.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://tcm.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jzw.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://cei.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fnp.fehbvm.com

[Q57] 行号
来源：http://ghu.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tnc.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://aot.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qnw.yuxming.cn

[Q59] 分组内累计
来源：http://geg.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rzz.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://hza.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vyh.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eee.hammf.cn

[Q61] 移动平均
来源：http://pre.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ddr.vqdsnc.cn

[Q62] 分组占比
来源：http://yhw.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ljb.yangfankeji.com

[Q63] 开启事务
来源：http://rkt.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ajq.ctjpmb.com

[Q64] 提交事务
来源：http://pwh.fanxiaobao.xyz

COMMIT;
来源：http://rxy.uphjek.com

[Q65] 回滚事务
来源：http://rin.ydzc1.top

ROLLBACK;
来源：http://lbc.zdqjudy.top

[Q66] 行锁查询
来源：http://hom.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jdc.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://qyj.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fdc.xuanzx.com

[Q68] 保存点
来源：http://lzb.wangdashe.top

SAVEPOINT sp1;
来源：http://mel.jyoumei.cn

ROLLBACK TO sp1;
来源：http://uyq.zhoulong.xyz

[Q69] 查看执行计划
来源：http://ppg.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cjb.jinqigfzy.top

[Q70] 更新统计信息
来源：http://nmr.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://gkr.aizwys.cn

[Q71] 查看建表语句
来源：http://wkp.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://snz.mhx1999.top

[Q72] 查看索引
来源：http://xdv.meibo888.top

SHOW INDEX FROM users;
来源：http://imq.haohaochexian.top

[Q73] 查看表状态
来源：http://evv.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wgz.sysykeji.top

[Q74] 强制使用索引
来源：http://vkf.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wqq.xuanzx.com

[Q75] 日期格式化
来源：http://aid.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rrd.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kyc.shuidangran.top

[Q76] 按天统计
来源：http://ezg.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hpq.uphjek.com

[Q77] 时间加减
来源：http://rqz.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uzl.yj20258.top

[Q78] 当前时间
来源：http://jza.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hjm.jinqigufen.top

[Q79] 字符串拼接
来源：http://ftc.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://apj.xylfe.cn

[Q80] 字符串截取
来源：http://aqi.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://alu.daxiang520.top

[Q81] 字符串替换
来源：http://iuv.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jcl.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://skl.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zcw.yj202588.top

[Q83] 大小写转换
来源：http://qei.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://idy.dashuyun.cn

[Q84] 去除首尾空格
来源：http://pjw.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://yhe.316326.xyz

[Q85] 数值取整
来源：http://hei.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pfw.ivvv.top

[Q86] 读取 JSON 字段
来源：http://ofq.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://myl.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://mre.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vwd.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://nvr.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zkr.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lze.smart0.xyz

[Q89] 判断表是否存在
来源：http://ueh.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qjp.shangyingyoupin.top

[Q90] 生成序号列
来源：http://geg.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wyh.tarul.cn

================================================================================
来源：http://jhu.fanxiaobao.xyz

R. Bash 专题
来源：http://eha.ehwqpu.com

================================================================================
来源：http://qhl.shzxlz.cn

[R01] shebang 与严格模式
来源：http://bte.zdbjq.cn

#!/usr/bin/env bash
来源：http://itn.ctjpmb.com

set -euo pipefail
来源：http://pqa.yueranfly.top

[R02] 变量赋值与使用
来源：http://uoy.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://wsb.gzhubu.top

[R03] 只读变量
来源：http://eri.cucudq.cn

readonly PI=3.14
来源：http://scy.cdnleiting.top

[R04] 位置参数
来源：http://hkc.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qep.ydzc1.top

[R05] 参数默认值
来源：http://oxt.wangdashe.top

name="${1:-default}"
来源：http://pgw.hysaishi.cn

[R06] 判断命令是否存在
来源：http://sry.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://icc.jyoumei.cn

[R07] if 判断文件
来源：http://erf.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://krj.sysykeji.top

[R08] 数值比较
来源：http://aln.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://keb.ivvv.top

[R09] 字符串比较
来源：http://qjb.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qod.ivvv.top

[R10] 正则匹配
来源：http://klr.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://umb.uphjek.com

[R11] case 多分支
来源：http://xro.xuanzx.com

case "$1" in
来源：http://cxj.sufxvd.cn

start) echo "启动" ;;
来源：http://met.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://rva.hesvh.cn

*)     echo "未知命令" ;;
来源：http://ufg.hongshengwenyu.top

esac
来源：http://ejn.ydjk.org.cn

[R12] for 遍历文件
来源：http://zsc.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://vqi.jinqigfzy.top

[R13] for 计数循环
来源：http://axk.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://fok.jyoumei.cn

[R14] C 风格 for
来源：http://aru.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vhh.fehbvm.com

[R15] while 逐行读文件
来源：http://ksm.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bek.ehwqpu.com

[R16] until 等待条件
来源：http://gxr.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jpb.xziqi.cn

[R17] 数组定义与取值
来源：http://ugt.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bxa.xuanzx.com

[R18] 遍历数组
来源：http://tpt.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ozn.hywenlv.cn

[R19] 数组长度
来源：http://pyd.gzhubu.top

echo "${#arr[@]}"
来源：http://ptf.shzxlz.cn

[R20] 关联数组（字典）
来源：http://zwr.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://glz.gogol.net.cn

[R21] 字符串长度
来源：http://ekc.zhaomingkeji.xyz

echo "${#s}"
来源：http://ihx.jinghuilouyu.cn

[R22] 截取子串
来源：http://knk.ppjwa.cn

echo "${s:0:5}"
来源：http://gzs.jinqigfzy.top

[R23] 字符串替换
来源：http://cau.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jfk.hysaishi.cn

[R24] 大小写转换
来源：http://pcg.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://btr.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://yqg.chenjidiqi.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://apk.gotoacloud.top

[R26] 命令替换
来源：http://tbc.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://mms.quarkkingdee.top

[R27] 算术展开
来源：http://djl.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://ntp.ivvv.top

[R28] 浮点运算
来源：http://vir.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://bic.ydjk.org.cn

[R29] 定义函数
来源：http://udz.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pcy.chenlongwang.top

[R30] 函数返回状态码
来源：http://pco.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://oxr.svipenyu.cn

[R31] 局部变量
来源：http://koh.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://msw.havefunace.top

[R32] 参数个数校验
来源：http://lpr.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yqb.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://nlv.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kpb.xylfe.cn

[R34] 退出时清理
来源：http://vmt.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://ljg.sysykeji.top

[R35] 后台执行并等待
来源：http://pip.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nce.hammf.cn

[R36] 并发执行多个任务
来源：http://xgg.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://osm.9152youxi.cn

[R37] 把输出赋给变量
来源：http://hai.xylfe.cn

files=$(ls -1)
来源：http://tjh.gogol.net.cn

[R38] 管道串联
来源：http://wvu.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://ezs.hammf.cn

[R39] 重定向标准输出与错误
来源：http://afy.yvedp.cn

cmd > out.log 2>&1
来源：http://gfv.gzhubu.top

[R40] 追加写日志
来源：http://gvy.hcnkem.com

echo "log" >> out.log
来源：http://qso.uphjek.com

[R41] 丢弃输出
来源：http://tlv.aibaodan.cn

cmd >/dev/null 2>&1
来源：http://rqh.guannengcc.top

[R42] 输入重定向
来源：http://usd.hongshengwenyu.top

wc -l < a.txt
来源：http://uwy.ybcxt.top

[R43] 按名字查找文件
来源：http://rnz.pycfn.com

find . -name "*.log" -type f
来源：http://mih.yj20258.top

[R44] 按修改时间查找
来源：http://bfv.hfpthk.cn

find . -mtime -7 -type f
来源：http://lny.fktsv.cn

[R45] 批量删除
来源：http://kdm.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://unv.iojbl.cn

[R46] 递归替换文件内容
来源：http://kos.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ccd.ydjk.org.cn

[R47] sed 单行替换
来源：http://fab.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://hka.birdmap.top

[R48] awk 取指定列
来源：http://xgp.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://sqx.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://cbl.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rqs.jinyuanbaomall.cn

[R50] awk 求和
来源：http://jjr.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://uct.fktsv.cn

[R51] 排序去重取前几
来源：http://wzz.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vzx.zhixingplan.top

[R52] 统计行数
来源：http://ijl.xuanzx.com

wc -l a.txt
来源：http://ltx.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://arl.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wpj.vehdjk.com

[R54] 比较两个文件
来源：http://yde.yongpay.top

diff a.txt b.txt
来源：http://orh.sufxvd.cn

[R55] 压缩与解压
来源：http://agd.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mvp.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://nog.uphjek.com

scp file user@host:/path/
来源：http://mlt.nanxuanxn.top

[R57] 远程执行命令
来源：http://evk.zdqjudy.top

ssh user@host 'uptime'
来源：http://uhl.zhengqikj.top

[R58] 下载文件
来源：http://bkk.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://osg.jianghu66.top

[R59] 发 POST JSON
来源：http://lez.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oow.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://ijy.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://thl.xinyue.icu

[R61] 磁盘占用
来源：http://gif.jqgufenzy.top

df -h;  du -sh *
来源：http://tpm.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://tbr.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://mlb.chenjidiqi.icu

[R63] 内存与进程
来源：http://ctk.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://nni.yonumen.top

[R64] 结束进程
来源：http://dka.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://ioi.gaohongyu789.top

[R65] 查看端口占用
来源：http://lqc.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ktp.ydzc1.top

[R66] 定时任务
来源：http://ipb.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://yyj.cashguo.top

[R67] 生成随机十六进制串
来源：http://glh.shanyushiyangtech.top

openssl rand -hex 16
来源：http://nfj.andypj.xyz

[R68] 计算文件校验值
来源：http://yyh.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qbk.yongpay.top

[R69] 生成随机密码
来源：http://kuu.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://hyp.vehdjk.com

[R70] 时间戳与互转
来源：http://eti.yuxming.cn

date +%s;  date -d @1700000000
来源：http://rqa.52xcode.cn

[R71] 日期格式化
来源：http://yrq.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ems.yuxming.cn

[R72] 等待端口就绪
来源：http://hmq.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hol.aizwys.cn

[R73] 分割大日志
来源：http://vxx.dianchejie.cn

split -l 1000 big.log part_
来源：http://fxq.redwolf501.top

[R74] 批量重命名
来源：http://wyc.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kbc.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://yfe.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://ukw.yfazqb.com

[R76] 使用临时文件
来源：http://cxq.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pqm.chenlongwang.top

[R77] 读取用户输入
来源：http://vqw.ehwqpu.com

read -rp "请输入: " ans
来源：http://eni.nanxinkj.top

[R78] 交互式菜单
来源：http://ayc.sufxvd.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oju.kuanghao11.cn

[R79] 解析命令行选项
来源：http://uun.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oiz.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://ick.pycfn.com

time ./run.sh
来源：http://rgk.9152youxi.cn

================================================================================
来源：http://xvh.aizwys.cn

S. C / C++ 专题
来源：http://jki.52xcode.cn

================================================================================
来源：http://vqn.hysaishi.cn

[S01] C：Hello World
来源：http://gpb.bbcook.cn

#include <stdio.h>
来源：http://adm.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://knp.birdmap.top

[S02] C：变量与格式化输出
来源：http://aff.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://xck.chenzaomai.com

[S03] C：读入整数
来源：http://azs.sysykeji.top

int x; scanf("%d", &x);
来源：http://jco.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://cuh.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://jmb.daxiang520.top

[S05] C：字符串长度
来源：http://wny.sufxvd.cn


<!-- 参考信息 -->