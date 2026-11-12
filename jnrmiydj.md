代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fab.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cxd.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eir.guowangkeji.top

[Q41] 多表连接
来源：http://syx.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oqn.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://cbg.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://ngl.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://xfp.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://pfv.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gbv.9152youxi.cn

[Q43] 标量子查询
来源：http://vbp.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://umt.0kj1m.cn

[Q44] IN 子查询
来源：http://mac.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://svb.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://yxc.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rgl.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hqp.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://szj.ehwqpu.com

[Q47] 与平均值比较
来源：http://sto.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nuh.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://ixq.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uyk.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://ghf.bbcook.cn

[Q49] 更新单行
来源：http://dvz.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bnm.daxiang520.top

[Q50] 批量更新
来源：http://rlk.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rrj.hfpthk.cn

[Q51] 用子查询更新
来源：http://fde.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://whz.redwolf501.top

[Q52] 删除指定行
来源：http://dfl.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://sjm.jianghu66.top

[Q53] 按条件删除
来源：http://nqo.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xov.hesvh.cn

[Q54] 清空表
来源：http://pyh.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://fqf.yfazqb.com

[Q55] 排名（并列占位）
来源：http://yji.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kqa.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://yqc.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kfh.aibaodan.cn

[Q57] 行号
来源：http://jzc.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bwh.fzhhl.top

[Q58] 累计求和
来源：http://kzg.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://irj.shangyingyoupin.top

[Q59] 分组内累计
来源：http://qoq.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jll.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://ije.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hxk.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cuf.cucudq.cn

[Q61] 移动平均
来源：http://hel.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ios.gzhubu.top

[Q62] 分组占比
来源：http://usz.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ndr.uphjek.com

[Q63] 开启事务
来源：http://snt.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xtq.yuanzhike.top

[Q64] 提交事务
来源：http://kqu.fktsv.cn

COMMIT;
来源：http://zik.bbcook.cn

[Q65] 回滚事务
来源：http://vez.hesvh.cn

ROLLBACK;
来源：http://baz.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://uvn.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wxo.meibo888.top

[Q67] 设置隔离级别
来源：http://dnc.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yvo.hammf.cn

[Q68] 保存点
来源：http://wie.sweek.top

SAVEPOINT sp1;
来源：http://xkf.52xcode.cn

ROLLBACK TO sp1;
来源：http://oqz.vqdsnc.cn

[Q69] 查看执行计划
来源：http://xlv.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bfc.gaohongyu789.top

[Q70] 更新统计信息
来源：http://npl.fzhhl.top

ANALYZE TABLE users;
来源：http://tgo.kuanghao11.cn

[Q71] 查看建表语句
来源：http://hvu.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bbv.bjfxy.top

[Q72] 查看索引
来源：http://uwf.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://mqg.52xcode.cn

[Q73] 查看表状态
来源：http://urj.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tbv.hfpthk.cn

[Q74] 强制使用索引
来源：http://ycl.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ebh.hfpthk.cn

[Q75] 日期格式化
来源：http://tpp.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dbk.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iyv.hongshengwenyu.top

[Q76] 按天统计
来源：http://cvm.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jgd.ybcxt.top

[Q77] 时间加减
来源：http://omn.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ixs.hesvh.cn

[Q78] 当前时间
来源：http://pzj.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ucd.yj20258888.top

[Q79] 字符串拼接
来源：http://pzl.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rts.tianlin.xyz

[Q80] 字符串截取
来源：http://why.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eyc.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://bzt.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pbo.tanke756.top

[Q82] 字符长度与字节长度
来源：http://kfg.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ghg.vehdjk.com

[Q83] 大小写转换
来源：http://rqw.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cuz.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://vxv.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://vvh.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://oeq.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://imk.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://kqd.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xma.zhijiandao.cn

[Q87] JSON 字段做条件
来源：http://isg.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zbs.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://qnn.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xlm.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qon.bjfxy.top

[Q89] 判断表是否存在
来源：http://wtl.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pmh.zycfv.cn

[Q90] 生成序号列
来源：http://snv.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rby.shzxlz.cn

================================================================================
来源：http://niz.jiagoushi.top

R. Bash 专题
来源：http://tpg.tanke756.top

================================================================================
来源：http://okt.0kj1m.cn

[R01] shebang 与严格模式
来源：http://mbu.hammf.cn

#!/usr/bin/env bash
来源：http://hqg.vehdjk.com

set -euo pipefail
来源：http://eft.daxiang520.top

[R02] 变量赋值与使用
来源：http://utz.havefunace.top

name="Tom"; echo "$name"
来源：http://uzd.ctjpmb.com

[R03] 只读变量
来源：http://rlw.yueranfly.top

readonly PI=3.14
来源：http://uwu.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://tic.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ugl.yuanzhike.top

[R05] 参数默认值
来源：http://ecy.hnqzz.top

name="${1:-default}"
来源：http://tbh.daxiang520.top

[R06] 判断命令是否存在
来源：http://nzt.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qbz.cqqwz.cn

[R07] if 判断文件
来源：http://ufz.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ord.yvedp.cn

[R08] 数值比较
来源：http://nqa.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mgg.jiagoushi.top

[R09] 字符串比较
来源：http://pfm.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nso.tarul.cn

[R10] 正则匹配
来源：http://jsz.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sdp.shanyushiyangtech.top

[R11] case 多分支
来源：http://vfm.zdbjq.cn

case "$1" in
来源：http://amf.sweek.top

start) echo "启动" ;;
来源：http://yuu.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://bbd.aizwys.cn

*)     echo "未知命令" ;;
来源：http://ezz.pycfn.com

esac
来源：http://hnr.andypj.xyz

[R12] for 遍历文件
来源：http://etm.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://cwr.tanke756.top

[R13] for 计数循环
来源：http://fyr.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://sfu.tianlin.xyz

[R14] C 风格 for
来源：http://uvf.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nwh.zhijiandao.cn

[R15] while 逐行读文件
来源：http://fsf.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fkl.shuidangran.top

[R16] until 等待条件
来源：http://dlj.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mqs.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://pty.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://poq.vehdjk.com

[R18] 遍历数组
来源：http://bqf.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uon.fehbvm.com

[R19] 数组长度
来源：http://ocm.gzhubu.top

echo "${#arr[@]}"
来源：http://itr.xylfe.cn

[R20] 关联数组（字典）
来源：http://jmj.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fqw.ybcxt.top

[R21] 字符串长度
来源：http://ste.shuidangran.top

echo "${#s}"
来源：http://ims.jqgufenzy.top

[R22] 截取子串
来源：http://xyk.ivvv.top

echo "${s:0:5}"
来源：http://qbs.gotoacloud.top

[R23] 字符串替换
来源：http://fud.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wzd.gzhubu.top

[R24] 大小写转换
来源：http://hji.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ekt.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://obo.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://asl.c1oappe.top

[R26] 命令替换
来源：http://jjc.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://vrg.hysaishi.cn

[R27] 算术展开
来源：http://vjy.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://yap.svipenyu.cn

[R28] 浮点运算
来源：http://nkr.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://jvm.zycfv.cn

[R29] 定义函数
来源：http://rgb.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fdq.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://ylp.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://wsf.yj20258.top

[R31] 局部变量
来源：http://nkt.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://obc.fzhhl.top

[R32] 参数个数校验
来源：http://gmh.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xcc.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://mso.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://smc.pengpengdd.cyou

[R34] 退出时清理
来源：http://jab.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vml.yueranfly.top

[R35] 后台执行并等待
来源：http://mto.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wvy.aizwys.cn

[R36] 并发执行多个任务
来源：http://iyz.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rvg.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://are.feifeiyinyue.top

files=$(ls -1)
来源：http://gca.yj202588.top

[R38] 管道串联
来源：http://djn.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://esk.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://syo.nwbrower.top

cmd > out.log 2>&1
来源：http://xgy.dianchejie.cn

[R40] 追加写日志
来源：http://wcb.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://mtg.yonumen.top

[R41] 丢弃输出
来源：http://nvl.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://gmn.dianchejie.cn

[R42] 输入重定向
来源：http://zvh.guowangkeji.top

wc -l < a.txt
来源：http://swb.jianghu66.top

[R43] 按名字查找文件
来源：http://wze.andypj.xyz

find . -name "*.log" -type f
来源：http://tzy.jyoumei.cn

[R44] 按修改时间查找
来源：http://utv.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://zwc.tanke756.top

[R45] 批量删除
来源：http://ygn.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://lsn.zhengqikj.top

[R46] 递归替换文件内容
来源：http://tkr.ehwqpu.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uud.yj202588.top

[R47] sed 单行替换
来源：http://gbn.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pqz.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://qtf.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://hrl.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://vkl.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mhh.pycfn.com

[R50] awk 求和
来源：http://vyg.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://arc.c1oappe.top

[R51] 排序去重取前几
来源：http://dvx.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://iwx.mhx1999.top

[R52] 统计行数
来源：http://zdi.dashuyun.cn

wc -l a.txt
来源：http://xcl.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://oyw.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yiz.yangfankeji.com

[R54] 比较两个文件
来源：http://vre.guannengcc.top

diff a.txt b.txt
来源：http://yph.ydjk.org.cn

[R55] 压缩与解压
来源：http://bnb.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wwd.wangshuangyany.cn

[R56] 远程拷贝
来源：http://xwd.yfazqb.com

scp file user@host:/path/
来源：http://xgx.nanxinkj.top

[R57] 远程执行命令
来源：http://kfl.haohaochexian.top

ssh user@host 'uptime'
来源：http://uzq.dashuyun.cn

[R58] 下载文件
来源：http://voz.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://spt.316326.xyz

[R59] 发 POST JSON
来源：http://cgh.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sor.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://irs.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tig.vqdsnc.cn

[R61] 磁盘占用
来源：http://doo.nwbrower.top

df -h;  du -sh *
来源：http://lfn.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://txf.yongpay.top

du -ah . | sort -rh | head -10
来源：http://tqi.gogol.net.cn

[R63] 内存与进程
来源：http://bpb.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://lwp.jqgfzy.top

[R64] 结束进程
来源：http://pva.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://ird.wangshuangyany.cn

[R65] 查看端口占用
来源：http://cny.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://erp.epnwcf.com

[R66] 定时任务
来源：http://toe.hnxiangtu.top

crontab -e;  crontab -l
来源：http://hnx.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://jiw.chenlongwang.top

openssl rand -hex 16
来源：http://hcv.hfpthk.cn

[R68] 计算文件校验值
来源：http://zxu.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://vqe.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://ecs.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://zpc.sysykeji.top

[R70] 时间戳与互转
来源：http://ssd.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://uqo.vehdjk.com

[R71] 日期格式化
来源：http://cyh.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yqv.havefunace.top

[R72] 等待端口就绪
来源：http://mps.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xkh.tarul.cn

[R73] 分割大日志
来源：http://plb.jianghu66.top

split -l 1000 big.log part_
来源：http://glm.andypj.xyz

[R74] 批量重命名
来源：http://vyq.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ioi.quarkkingdee.top

[R75] 导出环境变量
来源：http://aky.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://sjt.cdnleiting.top

[R76] 使用临时文件
来源：http://ibr.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://egx.shuidangran.top

[R77] 读取用户输入
来源：http://qcu.hfpthk.cn

read -rp "请输入: " ans
来源：http://ehr.iojbl.cn

[R78] 交互式菜单
来源：http://yvs.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jdo.ivvv.top

[R79] 解析命令行选项
来源：http://cqk.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xfc.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://weh.316326.xyz

time ./run.sh
来源：http://dug.hongshengwenyu.top

================================================================================
来源：http://qgc.hnqzz.top

S. C / C++ 专题
来源：http://zxe.yj20258888.top

================================================================================
来源：http://ieb.yuanzhike.top

[S01] C：Hello World
来源：http://piv.zhixingplan.top

#include <stdio.h>
来源：http://cln.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmx.fengsongda.top

[S02] C：变量与格式化输出
来源：http://eca.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://wee.9152youxi.cn

[S03] C：读入整数
来源：http://crv.yj20258888.top

int x; scanf("%d", &x);
来源：http://xez.xinyue.icu

[S04] C：字符串复制
来源：http://atd.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://jpr.jyoumei.cn

[S05] C：字符串长度
来源：http://mol.yongpay.top

strlen(s)
来源：http://blt.tian-w.cn

[S06] C：字符串比较
来源：http://mhy.316326.xyz

strcmp(a, b) == 0
来源：http://mff.yongpay.top

[S07] C：数组遍历求和
来源：http://tyk.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://igx.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://znn.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tdq.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://ttp.havefunace.top


<!-- 参考信息 -->