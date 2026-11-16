代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://vnn.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://arn.havefunace.top

[Q39] 自连接（查上下级）
来源：http://ioa.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://klu.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ssm.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rdi.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ans.guannengcc.top

[Q41] 多表连接
来源：http://dnb.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cvx.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://otv.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://bpf.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://pdc.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://zlp.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oho.guannengcc.top

[Q43] 标量子查询
来源：http://bxs.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sgn.sufxvd.cn

[Q44] IN 子查询
来源：http://gnc.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vqt.havefunace.top

[Q45] EXISTS 判断存在
来源：http://inc.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpi.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://nmt.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nyl.yanxiufei.cn

[Q47] 与平均值比较
来源：http://hqj.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jvq.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://xcl.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ofa.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ddb.yfazqb.com

[Q49] 更新单行
来源：http://pjd.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wri.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://xrr.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tsk.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://xln.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rjy.xuetiantiany.cn

[Q52] 删除指定行
来源：http://bcu.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://hmu.pycfn.com

[Q53] 按条件删除
来源：http://jdj.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tcs.jinqigufen.top

[Q54] 清空表
来源：http://mhg.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://hem.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://llo.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bfq.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://jfh.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vhj.quarkkingdee.top

[Q57] 行号
来源：http://gfy.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cdp.snrcjt.cn

[Q58] 累计求和
来源：http://wzu.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kxo.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://leh.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uly.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://pif.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cpg.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zfb.gotoacloud.top

[Q61] 移动平均
来源：http://xyf.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uxu.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://drs.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://muv.shanyushiyangtech.top

[Q63] 开启事务
来源：http://qlz.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nal.mhx1999.top

[Q64] 提交事务
来源：http://kyt.hfpthk.cn

COMMIT;
来源：http://shs.yongpay.top

[Q65] 回滚事务
来源：http://wsh.zhengqikj.top

ROLLBACK;
来源：http://wmo.gaohongyu789.top

[Q66] 行锁查询
来源：http://feu.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zon.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://sye.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nit.ivvv.top

[Q68] 保存点
来源：http://mkz.ybcxt.top

SAVEPOINT sp1;
来源：http://zdl.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://rky.zdqjudy.top

[Q69] 查看执行计划
来源：http://mig.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kcn.epnwcf.com

[Q70] 更新统计信息
来源：http://ntg.hnxiangtu.top

ANALYZE TABLE users;
来源：http://smy.jinqigfzy.top

[Q71] 查看建表语句
来源：http://vyh.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vwl.jqgufenzy.top

[Q72] 查看索引
来源：http://ttb.yangfankeji.com

SHOW INDEX FROM users;
来源：http://uwj.fktsv.cn

[Q73] 查看表状态
来源：http://weh.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hjj.aibaodan.cn

[Q74] 强制使用索引
来源：http://hsn.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eec.nwbrower.top

[Q75] 日期格式化
来源：http://hpf.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nqv.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nmo.jyoumei.cn

[Q76] 按天统计
来源：http://ryb.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://udq.yj20258.top

[Q77] 时间加减
来源：http://xpx.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zlh.jqgfzy.top

[Q78] 当前时间
来源：http://cdw.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jtn.aizwys.cn

[Q79] 字符串拼接
来源：http://zvo.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xqt.shuidangran.top

[Q80] 字符串截取
来源：http://fgu.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rfu.guowangkeji.top

[Q81] 字符串替换
来源：http://ofj.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gzg.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://img.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fha.jqgfzy.top

[Q83] 大小写转换
来源：http://lwt.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iqo.zycfv.cn

[Q84] 去除首尾空格
来源：http://qoo.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://mnw.yj20258.top

[Q85] 数值取整
来源：http://phy.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jie.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://hoq.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bbg.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://zzo.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gwo.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://wxg.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wnz.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wur.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://vme.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uhh.hywenlv.cn

[Q90] 生成序号列
来源：http://toc.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uop.guowangkeji.top

================================================================================
来源：http://qli.fktsv.cn

R. Bash 专题
来源：http://hif.dianchejie.cn

================================================================================
来源：http://fsr.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://kzx.sxryk.cn

#!/usr/bin/env bash
来源：http://ddt.c1oappe.top

set -euo pipefail
来源：http://xxc.jiagoushi.top

[R02] 变量赋值与使用
来源：http://qwc.jianghu66.top

name="Tom"; echo "$name"
来源：http://jwn.tian-w.cn

[R03] 只读变量
来源：http://eow.fanxiaobao.xyz

readonly PI=3.14
来源：http://jzk.birdmap.top

[R04] 位置参数
来源：http://ari.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qas.nwbrower.top

[R05] 参数默认值
来源：http://vhy.havefunace.top

name="${1:-default}"
来源：http://zmk.chenlongwang.top

[R06] 判断命令是否存在
来源：http://qtj.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nwv.svipenyu.cn

[R07] if 判断文件
来源：http://odt.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fwa.wangshuangyany.cn

[R08] 数值比较
来源：http://wmy.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fyd.ctjpmb.com

[R09] 字符串比较
来源：http://lot.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mhl.haohaochexian.top

[R10] 正则匹配
来源：http://zpf.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://izz.tianlin.xyz

[R11] case 多分支
来源：http://urz.xingfuxueyuan.xyz

case "$1" in
来源：http://uja.wangshuangyany.cn

start) echo "启动" ;;
来源：http://gaw.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://wir.sweek.top

*)     echo "未知命令" ;;
来源：http://hbo.ctjpmb.com

esac
来源：http://qsu.ydjk.org.cn

[R12] for 遍历文件
来源：http://fkl.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://ncq.hywenlv.cn

[R13] for 计数循环
来源：http://rem.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://axw.meibo888.top

[R14] C 风格 for
来源：http://asi.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nim.redwolf501.top

[R15] while 逐行读文件
来源：http://qxf.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cgh.feifeiyinyue.top

[R16] until 等待条件
来源：http://oal.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iij.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://pkx.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://cdr.cqqwz.cn

[R18] 遍历数组
来源：http://mcs.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zrj.cucudq.cn

[R19] 数组长度
来源：http://kjd.sufxvd.cn

echo "${#arr[@]}"
来源：http://hls.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://tvd.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yze.hcnkem.com

[R21] 字符串长度
来源：http://xpl.birdmap.top

echo "${#s}"
来源：http://qoa.ppjwa.cn

[R22] 截取子串
来源：http://duk.guowangkeji.top

echo "${s:0:5}"
来源：http://gbd.sjlbkw.cn

[R23] 字符串替换
来源：http://kwi.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gdj.hesvh.cn

[R24] 大小写转换
来源：http://uwo.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rrz.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://cdy.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bul.feifeiyinyue.top

[R26] 命令替换
来源：http://ebw.tarul.cn

now=$(date +%F); echo "$now"
来源：http://gia.ydjk.org.cn

[R27] 算术展开
来源：http://jxn.yj20258888.top

echo $((1 + 2 * 3))
来源：http://wvu.zhijiandao.cn

[R28] 浮点运算
来源：http://qyj.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://ocn.yvedp.cn

[R29] 定义函数
来源：http://vim.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://buu.ybcxt.top

[R30] 函数返回状态码
来源：http://tts.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://lmc.pengpengdd.cyou

[R31] 局部变量
来源：http://ono.sweek.top

f() { local x=1; echo "$x"; }
来源：http://gui.sweek.top

[R32] 参数个数校验
来源：http://uph.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qqo.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://igg.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lbt.xziqi.cn

[R34] 退出时清理
来源：http://xqn.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://luz.zhixingplan.top

[R35] 后台执行并等待
来源：http://oqd.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://das.aibaodan.cn

[R36] 并发执行多个任务
来源：http://wsy.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vqz.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://xfw.hongshengwenyu.top

files=$(ls -1)
来源：http://tog.yj202588.top

[R38] 管道串联
来源：http://odw.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://qgu.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://daq.snrcjt.cn

cmd > out.log 2>&1
来源：http://lth.yangfankeji.com

[R40] 追加写日志
来源：http://mnd.feifeiyinyue.top

echo "log" >> out.log
来源：http://qrc.sxryk.cn

[R41] 丢弃输出
来源：http://lqu.316326.xyz

cmd >/dev/null 2>&1
来源：http://qsv.hcnkem.com

[R42] 输入重定向
来源：http://qaq.snrcjt.cn

wc -l < a.txt
来源：http://rsj.snrcjt.cn

[R43] 按名字查找文件
来源：http://oxt.guannengcc.top

find . -name "*.log" -type f
来源：http://frm.yongpay.top

[R44] 按修改时间查找
来源：http://ajd.9152youxi.cn

find . -mtime -7 -type f
来源：http://mjx.ydjk.org.cn

[R45] 批量删除
来源：http://raw.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://clg.sweek.top

[R46] 递归替换文件内容
来源：http://dpo.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://avv.shuidangran.top

[R47] sed 单行替换
来源：http://fuz.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://wzj.yfazqb.com

[R48] awk 取指定列
来源：http://cpv.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://mix.ehwqpu.com

[R49] awk 带条件
来源：http://ovx.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xiz.gotoacloud.top

[R50] awk 求和
来源：http://uqh.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://lxg.yj20258888.top

[R51] 排序去重取前几
来源：http://xwq.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ayt.redwolf501.top

[R52] 统计行数
来源：http://mjw.zhoulong.xyz

wc -l a.txt
来源：http://gfa.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://nxk.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uqx.0kj1m.cn

[R54] 比较两个文件
来源：http://mcd.sysykeji.top

diff a.txt b.txt
来源：http://ffb.zhijiandao.cn

[R55] 压缩与解压
来源：http://jnt.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dls.hcnkem.com

[R56] 远程拷贝
来源：http://hmu.hammf.cn

scp file user@host:/path/
来源：http://luw.9152youxi.cn

[R57] 远程执行命令
来源：http://jhh.bjfxy.top

ssh user@host 'uptime'
来源：http://qlz.ppjwa.cn

[R58] 下载文件
来源：http://vcb.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eig.guannengcc.top

[R59] 发 POST JSON
来源：http://kag.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nwg.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://qos.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cfn.pycfn.com

[R61] 磁盘占用
来源：http://riu.hongshengwenyu.top

df -h;  du -sh *
来源：http://yaw.sysykeji.top

[R62] 找最占空间的文件
来源：http://qao.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://lhj.xylfe.cn

[R63] 内存与进程
来源：http://wgn.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://ujf.gogol.net.cn

[R64] 结束进程
来源：http://caa.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://fpz.cucudq.cn

[R65] 查看端口占用
来源：http://uak.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pzb.hywenlv.cn

[R66] 定时任务
来源：http://yoq.quarkkingdee.top

crontab -e;  crontab -l
来源：http://ucq.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://zpe.ybcxt.top

openssl rand -hex 16
来源：http://nes.svipenyu.cn

[R68] 计算文件校验值
来源：http://ofm.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://ypt.cqqwz.cn

[R69] 生成随机密码
来源：http://rgq.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://bbd.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://uib.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://hqd.nanxuanxn.top

[R71] 日期格式化
来源：http://pzj.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://awa.aibaodan.cn

[R72] 等待端口就绪
来源：http://mxw.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qty.hcnkem.com

[R73] 分割大日志
来源：http://xyu.fktsv.cn

split -l 1000 big.log part_
来源：http://lqf.hnqzz.top

[R74] 批量重命名
来源：http://kcz.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nfa.cheryme.top

[R75] 导出环境变量
来源：http://zba.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://zrg.yonumen.top

[R76] 使用临时文件
来源：http://pyj.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fiy.nwbrower.top

[R77] 读取用户输入
来源：http://uql.zhengqikj.top

read -rp "请输入: " ans
来源：http://fph.epnwcf.com

[R78] 交互式菜单
来源：http://xnb.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://trv.hesvh.cn

[R79] 解析命令行选项
来源：http://kde.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cup.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://yls.shangyingyoupin.top

time ./run.sh
来源：http://fsc.zdqjudy.top

================================================================================
来源：http://tkw.hysaishi.cn

S. C / C++ 专题
来源：http://eki.dianchejie.cn

================================================================================
来源：http://umb.tian-w.cn

[S01] C：Hello World
来源：http://olm.xinyue.icu

#include <stdio.h>
来源：http://gze.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://gju.ydzc1.top

[S02] C：变量与格式化输出
来源：http://yel.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://sti.gzhubu.top

[S03] C：读入整数
来源：http://zjw.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://uhh.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://sgy.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://sao.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://lci.52xcode.cn

strlen(s)
来源：http://uyz.chenlongwang.top

[S06] C：字符串比较
来源：http://hbw.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://hsr.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://teg.yuanzhike.top


<!-- 参考信息 -->