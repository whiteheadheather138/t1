代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://xfu.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oqx.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://pak.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lfe.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://stz.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wpb.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://djo.zhiwuduotai.top

[Q41] 多表连接
来源：http://flx.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://htm.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://erw.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://fjm.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://yoa.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://uzx.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fhz.birdmap.top

[Q43] 标量子查询
来源：http://hmm.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cbe.ctjpmb.com

[Q44] IN 子查询
来源：http://lcm.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kgl.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://vvd.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oyf.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rhf.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ybl.yongpay.top

[Q47] 与平均值比较
来源：http://fhx.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bih.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://slt.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wzh.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://mnv.cqqwz.cn

[Q49] 更新单行
来源：http://dhp.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://txt.zhixingplan.top

[Q50] 批量更新
来源：http://qmf.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lxy.vqdsnc.cn

[Q51] 用子查询更新
来源：http://vjq.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iut.dashuyun.cn

[Q52] 删除指定行
来源：http://tht.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://uem.gotoacloud.top

[Q53] 按条件删除
来源：http://gce.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qqy.sxryk.cn

[Q54] 清空表
来源：http://qgu.yvedp.cn

TRUNCATE TABLE logs;
来源：http://csg.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://aeg.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gay.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://ucn.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://edc.yongpay.top

[Q57] 行号
来源：http://cdd.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qlx.cheryme.top

[Q58] 累计求和
来源：http://qcr.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://api.yonumen.top

[Q59] 分组内累计
来源：http://beg.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kkf.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://ymw.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nyo.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yqx.hywenlv.cn

[Q61] 移动平均
来源：http://fnb.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kwy.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://uid.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xoe.nanxinkj.top

[Q63] 开启事务
来源：http://xpp.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ubb.shuidangran.top

[Q64] 提交事务
来源：http://jyi.sysykeji.top

COMMIT;
来源：http://hiv.daxiang520.top

[Q65] 回滚事务
来源：http://cql.yfazqb.com

ROLLBACK;
来源：http://eni.svipenyu.cn

[Q66] 行锁查询
来源：http://sub.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wny.uphjek.com

[Q67] 设置隔离级别
来源：http://cje.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ovz.jqgfzy.top

[Q68] 保存点
来源：http://lsu.fzhhl.top

SAVEPOINT sp1;
来源：http://yvl.jiagoushi.top

ROLLBACK TO sp1;
来源：http://ycw.haohaochexian.top

[Q69] 查看执行计划
来源：http://nsh.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://htq.bbcook.cn

[Q70] 更新统计信息
来源：http://aaq.zycfv.cn

ANALYZE TABLE users;
来源：http://nkl.jianghu66.top

[Q71] 查看建表语句
来源：http://pdq.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mxv.yanxiufei.cn

[Q72] 查看索引
来源：http://zff.xziqi.cn

SHOW INDEX FROM users;
来源：http://htx.zhoulong.xyz

[Q73] 查看表状态
来源：http://ltf.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kki.cheryme.top

[Q74] 强制使用索引
来源：http://why.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rlq.haohaochexian.top

[Q75] 日期格式化
来源：http://wmn.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tqt.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gaz.c1oappe.top

[Q76] 按天统计
来源：http://whl.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ylf.gogol.net.cn

[Q77] 时间加减
来源：http://uxd.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xgk.zdqjudy.top

[Q78] 当前时间
来源：http://hpt.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ari.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://zwa.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rfe.ivvv.top

[Q80] 字符串截取
来源：http://yec.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gvw.bjfxy.top

[Q81] 字符串替换
来源：http://amu.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ysc.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://itd.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yyr.guowangkeji.top

[Q83] 大小写转换
来源：http://gcs.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ryz.ydzc1.top

[Q84] 去除首尾空格
来源：http://lub.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://vsb.xinyue.icu

[Q85] 数值取整
来源：http://mgs.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bao.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://jdl.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nru.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://sen.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://avx.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://bmn.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vcq.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ubw.0kj1m.cn

[Q89] 判断表是否存在
来源：http://tyz.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcc.snrcjt.cn

[Q90] 生成序号列
来源：http://sgi.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wow.hfpthk.cn

================================================================================
来源：http://tqi.pycfn.com

R. Bash 专题
来源：http://pxk.hfpthk.cn

================================================================================
来源：http://qdp.vehdjk.com

[R01] shebang 与严格模式
来源：http://lqx.bjfxy.top

#!/usr/bin/env bash
来源：http://qbs.ctjpmb.com

set -euo pipefail
来源：http://uvk.andypj.xyz

[R02] 变量赋值与使用
来源：http://bfp.9152youxi.cn

name="Tom"; echo "$name"
来源：http://odp.yvedp.cn

[R03] 只读变量
来源：http://gag.9152youxi.cn

readonly PI=3.14
来源：http://kyc.hongshengwenyu.top

[R04] 位置参数
来源：http://czq.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vvy.tarul.cn

[R05] 参数默认值
来源：http://xta.feifeiyinyue.top

name="${1:-default}"
来源：http://pau.sweek.top

[R06] 判断命令是否存在
来源：http://qzk.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://epv.smart0.xyz

[R07] if 判断文件
来源：http://svc.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xdh.gaohongyu789.top

[R08] 数值比较
来源：http://hoy.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gig.sjlbkw.cn

[R09] 字符串比较
来源：http://kzq.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://caw.havefunace.top

[R10] 正则匹配
来源：http://zsg.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uox.feifeiyinyue.top

[R11] case 多分支
来源：http://iaw.aizwys.cn

case "$1" in
来源：http://nym.c1oappe.top

start) echo "启动" ;;
来源：http://yqy.aizwys.cn

stop)  echo "停止" ;;
来源：http://xft.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://owj.bjfxy.top

esac
来源：http://zsp.uphjek.com

[R12] for 遍历文件
来源：http://yxr.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://qiv.zhongyouzk.top

[R13] for 计数循环
来源：http://zbl.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://msw.snrcjt.cn

[R14] C 风格 for
来源：http://ckf.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nvd.snrcjt.cn

[R15] while 逐行读文件
来源：http://lmy.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vjb.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://ixb.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://thh.sysykeji.top

[R17] 数组定义与取值
来源：http://elh.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://qoo.ivvv.top

[R18] 遍历数组
来源：http://sov.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://igj.tanke756.top

[R19] 数组长度
来源：http://axl.andypj.xyz

echo "${#arr[@]}"
来源：http://esr.hnqzz.top

[R20] 关联数组（字典）
来源：http://rhr.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ckh.andypj.xyz

[R21] 字符串长度
来源：http://cur.vqdsnc.cn

echo "${#s}"
来源：http://vkc.tarul.cn

[R22] 截取子串
来源：http://jvu.vehdjk.com

echo "${s:0:5}"
来源：http://eao.fanxiaobao.xyz

[R23] 字符串替换
来源：http://kxi.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gsk.meibo888.top

[R24] 大小写转换
来源：http://nii.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://qmp.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://mez.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uqd.zhaomingkeji.xyz

[R26] 命令替换
来源：http://bqr.birdmap.top

now=$(date +%F); echo "$now"
来源：http://qpu.ydjk.org.cn

[R27] 算术展开
来源：http://tim.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://ruk.zdqjudy.top

[R28] 浮点运算
来源：http://mfv.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://aon.zhiwuduotai.top

[R29] 定义函数
来源：http://eob.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qge.sysykeji.top

[R30] 函数返回状态码
来源：http://tds.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://xmg.svipenyu.cn

[R31] 局部变量
来源：http://upw.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://jzx.hywenlv.cn

[R32] 参数个数校验
来源：http://yca.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jhb.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://efq.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gkf.yanxiufei.cn

[R34] 退出时清理
来源：http://mmu.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://wbr.hywenlv.cn

[R35] 后台执行并等待
来源：http://dkv.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qhl.yj20258.top

[R36] 并发执行多个任务
来源：http://qwk.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zkv.cucudq.cn

[R37] 把输出赋给变量
来源：http://xft.yj20258.top

files=$(ls -1)
来源：http://csi.aibaodan.cn

[R38] 管道串联
来源：http://prn.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://asl.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://vmc.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://ujl.dianchejie.cn

[R40] 追加写日志
来源：http://yuk.zhixingplan.top

echo "log" >> out.log
来源：http://ozw.chenjidiqi.icu

[R41] 丢弃输出
来源：http://rjd.wangdashe.top

cmd >/dev/null 2>&1
来源：http://oih.tanke756.top

[R42] 输入重定向
来源：http://ytn.shangyingyoupin.top

wc -l < a.txt
来源：http://izg.ydjk.org.cn

[R43] 按名字查找文件
来源：http://fmb.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://yfy.c1oappe.top

[R44] 按修改时间查找
来源：http://emg.hcnkem.com

find . -mtime -7 -type f
来源：http://ksu.pycfn.com

[R45] 批量删除
来源：http://uqw.birdmap.top

find . -name "*.tmp" -delete
来源：http://edc.zdbjq.cn

[R46] 递归替换文件内容
来源：http://arj.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xdt.daria6918.cn

[R47] sed 单行替换
来源：http://gli.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mhv.316326.xyz

[R48] awk 取指定列
来源：http://nbe.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://dgb.wangshuangyany.cn

[R49] awk 带条件
来源：http://isw.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jvt.hongshengwenyu.top

[R50] awk 求和
来源：http://mnn.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ybk.ydjk.org.cn

[R51] 排序去重取前几
来源：http://gyc.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://nje.daria6918.cn

[R52] 统计行数
来源：http://ohr.chenjidiqi.icu

wc -l a.txt
来源：http://fnc.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://frh.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zhs.shuidangran.top

[R54] 比较两个文件
来源：http://huz.nanxuanxn.top

diff a.txt b.txt
来源：http://cqe.aibaodan.cn

[R55] 压缩与解压
来源：http://nhv.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rok.yj20258888.top

[R56] 远程拷贝
来源：http://yie.chenjidiqi.icu

scp file user@host:/path/
来源：http://dfr.xuanzx.com

[R57] 远程执行命令
来源：http://grm.epnwcf.com

ssh user@host 'uptime'
来源：http://vnu.c1oappe.top

[R58] 下载文件
来源：http://atj.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dmx.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://uzy.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://enn.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://kxq.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uyd.fzhhl.top

[R61] 磁盘占用
来源：http://hzg.c1oappe.top

df -h;  du -sh *
来源：http://buc.aizwys.cn

[R62] 找最占空间的文件
来源：http://zyq.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://mzs.jlsjyb.cn

[R63] 内存与进程
来源：http://uni.ivvv.top

free -h;  ps aux | grep nginx
来源：http://zcp.316326.xyz

[R64] 结束进程
来源：http://lpi.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://lvl.jinqigufen.top

[R65] 查看端口占用
来源：http://rmd.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://spw.cheryme.top

[R66] 定时任务
来源：http://ypl.aizwys.cn

crontab -e;  crontab -l
来源：http://aou.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://jpq.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://xty.bbcook.cn

[R68] 计算文件校验值
来源：http://ilu.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://mfz.cqqwz.cn

[R69] 生成随机密码
来源：http://shf.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://duh.snrcjt.cn

[R70] 时间戳与互转
来源：http://kve.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://exe.jinghuilouyu.cn

[R71] 日期格式化
来源：http://qen.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oeh.zhijiandao.cn

[R72] 等待端口就绪
来源：http://oas.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://mnm.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://pdh.xylfe.cn

split -l 1000 big.log part_
来源：http://vdw.haohaochexian.top

[R74] 批量重命名
来源：http://qmg.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mjo.xziqi.cn

[R75] 导出环境变量
来源：http://vql.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://oxk.daria6918.cn

[R76] 使用临时文件
来源：http://lgx.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jqu.daxiang520.top

[R77] 读取用户输入
来源：http://wij.52xcode.cn

read -rp "请输入: " ans
来源：http://exo.sjlbkw.cn

[R78] 交互式菜单
来源：http://fpn.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yzo.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://ebr.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lvw.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://erz.zdbjq.cn

time ./run.sh
来源：http://gjx.yuanzhike.top

================================================================================
来源：http://kox.ybcxt.top

S. C / C++ 专题
来源：http://jdm.jyoumei.cn

================================================================================
来源：http://eeh.pengpengdd.cyou

[S01] C：Hello World
来源：http://flo.zhiwuduotai.top

#include <stdio.h>
来源：http://iyx.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rpy.jianghu66.top

[S02] C：变量与格式化输出
来源：http://lzo.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://iir.guowangkeji.top

[S03] C：读入整数
来源：http://quo.cqqwz.cn

int x; scanf("%d", &x);
来源：http://zkk.snrcjt.cn

[S04] C：字符串复制
来源：http://mzo.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ggi.shangyingyoupin.top

[S05] C：字符串长度
来源：http://ejj.jlsjyb.cn

strlen(s)
来源：http://nwj.svipenyu.cn

[S06] C：字符串比较
来源：http://axm.yj20258888.top

strcmp(a, b) == 0
来源：http://lwv.smart0.xyz

[S07] C：数组遍历求和
来源：http://cgw.chenzaomai.com


<!-- 参考信息 -->