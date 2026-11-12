代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://orm.hfpthk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fml.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dtf.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://bsq.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hqv.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://wes.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://bzs.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://pas.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://izw.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zmr.yj20258888.top

[Q43] 标量子查询
来源：http://cqr.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pgx.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://oup.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xcx.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://tzt.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sux.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://tur.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://asb.pycfn.com

[Q47] 与平均值比较
来源：http://mdq.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cps.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://npw.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://szr.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://uhc.jlsjyb.cn

[Q49] 更新单行
来源：http://cxl.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vwa.pengpengdd.cyou

[Q50] 批量更新
来源：http://jrp.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ctm.wangdashe.top

[Q51] 用子查询更新
来源：http://dyy.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fqe.jlsjyb.cn

[Q52] 删除指定行
来源：http://ulf.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://vck.chenzaomai.com

[Q53] 按条件删除
来源：http://qbm.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yeh.andypj.xyz

[Q54] 清空表
来源：http://lrd.shuidangran.top

TRUNCATE TABLE logs;
来源：http://awp.tian-w.cn

[Q55] 排名（并列占位）
来源：http://mea.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hyd.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://kke.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bet.yj20258888.top

[Q57] 行号
来源：http://clo.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bbb.yj202588.top

[Q58] 累计求和
来源：http://uso.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mgw.dianchejie.cn

[Q59] 分组内累计
来源：http://vgb.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wmx.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://tyv.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sgv.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://exb.chenjidiqi.icu

[Q61] 移动平均
来源：http://fpm.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wwb.zhijiandao.cn

[Q62] 分组占比
来源：http://ycy.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://msb.shanyushiyangtech.top

[Q63] 开启事务
来源：http://rix.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://pez.svipenyu.cn

[Q64] 提交事务
来源：http://flz.chenlongwang.top

COMMIT;
来源：http://qqc.fehbvm.com

[Q65] 回滚事务
来源：http://gqb.nwbrower.top

ROLLBACK;
来源：http://lqz.yonumen.top

[Q66] 行锁查询
来源：http://ygb.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qrt.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://wds.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gmt.zhijiandao.cn

[Q68] 保存点
来源：http://hjt.bbcook.cn

SAVEPOINT sp1;
来源：http://fhx.hammf.cn

ROLLBACK TO sp1;
来源：http://lqh.316326.xyz

[Q69] 查看执行计划
来源：http://awl.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iht.fehbvm.com

[Q70] 更新统计信息
来源：http://aog.ctjpmb.com

ANALYZE TABLE users;
来源：http://rxy.chenlongwang.top

[Q71] 查看建表语句
来源：http://ctd.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xwf.nwbrower.top

[Q72] 查看索引
来源：http://ayl.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://wok.cheryme.top

[Q73] 查看表状态
来源：http://rkc.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rmb.birdmap.top

[Q74] 强制使用索引
来源：http://cnh.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jqs.fehbvm.com

[Q75] 日期格式化
来源：http://nft.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dlh.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://soo.tarul.cn

[Q76] 按天统计
来源：http://whf.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kpv.snrcjt.cn

[Q77] 时间加减
来源：http://yfn.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nrk.shanyushiyangtech.top

[Q78] 当前时间
来源：http://dwc.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gko.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://fiz.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lvh.ctjpmb.com

[Q80] 字符串截取
来源：http://hbd.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wjh.aizwys.cn

[Q81] 字符串替换
来源：http://okr.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hjt.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://eqq.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://flp.ppjwa.cn

[Q83] 大小写转换
来源：http://zrr.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jza.sysykeji.top

[Q84] 去除首尾空格
来源：http://ifx.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://jxu.chenzaomai.com

[Q85] 数值取整
来源：http://jfy.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tyq.meibo888.top

[Q86] 读取 JSON 字段
来源：http://lsc.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lwz.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://onh.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wyi.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://oah.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kpo.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zfz.iojbl.cn

[Q89] 判断表是否存在
来源：http://smb.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://efs.jyoumei.cn

[Q90] 生成序号列
来源：http://nif.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cbd.yonumen.top

================================================================================
来源：http://xks.tanke756.top

R. Bash 专题
来源：http://avv.vehdjk.com

================================================================================
来源：http://wuk.c1oappe.top

[R01] shebang 与严格模式
来源：http://wmj.hcnkem.com

#!/usr/bin/env bash
来源：http://luj.ctjpmb.com

set -euo pipefail
来源：http://ome.0kj1m.cn

[R02] 变量赋值与使用
来源：http://ovm.chenlongwang.top

name="Tom"; echo "$name"
来源：http://zaq.xinyue.icu

[R03] 只读变量
来源：http://oxz.gogol.net.cn

readonly PI=3.14
来源：http://toj.cheryme.top

[R04] 位置参数
来源：http://iya.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pts.fengsongda.top

[R05] 参数默认值
来源：http://ikk.jyoumei.cn

name="${1:-default}"
来源：http://cpb.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://bbr.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ouc.xuetiantiany.cn

[R07] if 判断文件
来源：http://tfc.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhv.yuxming.cn

[R08] 数值比较
来源：http://ihc.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sbf.yfazqb.com

[R09] 字符串比较
来源：http://toc.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://emx.ivvv.top

[R10] 正则匹配
来源：http://oxh.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iae.nanxuanxn.top

[R11] case 多分支
来源：http://jun.tian-w.cn

case "$1" in
来源：http://tav.ydzc1.top

start) echo "启动" ;;
来源：http://ztr.yj20258888.top

stop)  echo "停止" ;;
来源：http://abk.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://wnk.xinyue.icu

esac
来源：http://xhn.zdbjq.cn

[R12] for 遍历文件
来源：http://pkt.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://xdk.mhx1999.top

[R13] for 计数循环
来源：http://esx.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://qzx.sysykeji.top

[R14] C 风格 for
来源：http://paf.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dul.gaohongyu789.top

[R15] while 逐行读文件
来源：http://khp.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mzk.zhijiandao.cn

[R16] until 等待条件
来源：http://wuz.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://brg.316326.xyz

[R17] 数组定义与取值
来源：http://acw.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://ssz.zhongyouzk.top

[R18] 遍历数组
来源：http://xmd.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://koh.xylfe.cn

[R19] 数组长度
来源：http://qid.yongpay.top

echo "${#arr[@]}"
来源：http://ybi.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://sbg.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vfw.cdnleiting.top

[R21] 字符串长度
来源：http://smi.pengpengdd.cyou

echo "${#s}"
来源：http://kmm.feifeiyinyue.top

[R22] 截取子串
来源：http://rsc.cheryme.top

echo "${s:0:5}"
来源：http://isc.hesvh.cn

[R23] 字符串替换
来源：http://loe.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://anv.bjfxy.top

[R24] 大小写转换
来源：http://fxb.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://iwz.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://zhn.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yce.hnqzz.top

[R26] 命令替换
来源：http://gpu.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://uwk.cashguo.top

[R27] 算术展开
来源：http://ltj.cashguo.top

echo $((1 + 2 * 3))
来源：http://fal.ppjwa.cn

[R28] 浮点运算
来源：http://xik.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://vkv.cheryme.top

[R29] 定义函数
来源：http://ndb.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ote.vehdjk.com

[R30] 函数返回状态码
来源：http://teq.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://osr.nanxinkj.top

[R31] 局部变量
来源：http://qis.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://lkh.feifeiyinyue.top

[R32] 参数个数校验
来源：http://qko.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nqv.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://azi.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rwy.hywenlv.cn

[R34] 退出时清理
来源：http://vlh.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://gmf.zdqjudy.top

[R35] 后台执行并等待
来源：http://zjb.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://enx.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://vjb.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sev.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://qet.bjfxy.top

files=$(ls -1)
来源：http://vsj.tian-w.cn

[R38] 管道串联
来源：http://son.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://lry.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://wxo.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://aqm.fktsv.cn

[R40] 追加写日志
来源：http://dvl.hysaishi.cn

echo "log" >> out.log
来源：http://ils.nanxinkj.top

[R41] 丢弃输出
来源：http://rfb.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://dbx.yanxiufei.cn

[R42] 输入重定向
来源：http://wuc.hammf.cn

wc -l < a.txt
来源：http://htr.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://pmq.pycfn.com

find . -name "*.log" -type f
来源：http://tla.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://vcw.316326.xyz

find . -mtime -7 -type f
来源：http://ceo.bbcook.cn

[R45] 批量删除
来源：http://ims.cashguo.top

find . -name "*.tmp" -delete
来源：http://awp.hnqzz.top

[R46] 递归替换文件内容
来源：http://ljh.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zrq.haohaochexian.top

[R47] sed 单行替换
来源：http://lyt.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://ksb.ppjwa.cn

[R48] awk 取指定列
来源：http://tyx.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://cno.yvedp.cn

[R49] awk 带条件
来源：http://ohe.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vlv.yuxming.cn

[R50] awk 求和
来源：http://zbv.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://wdo.ctjpmb.com

[R51] 排序去重取前几
来源：http://dao.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fqx.xylfe.cn

[R52] 统计行数
来源：http://ysa.yanxiufei.cn

wc -l a.txt
来源：http://mce.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://kxb.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bhx.0kj1m.cn

[R54] 比较两个文件
来源：http://xjt.chenlongwang.top

diff a.txt b.txt
来源：http://mjq.zycfv.cn

[R55] 压缩与解压
来源：http://osm.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ccy.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://nla.hesvh.cn

scp file user@host:/path/
来源：http://xce.xylfe.cn

[R57] 远程执行命令
来源：http://irv.yj20258.top

ssh user@host 'uptime'
来源：http://kip.fehbvm.com

[R58] 下载文件
来源：http://tdi.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yoq.smart0.xyz

[R59] 发 POST JSON
来源：http://nwy.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://stk.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://puk.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hgd.sufxvd.cn

[R61] 磁盘占用
来源：http://whv.jianghu66.top

df -h;  du -sh *
来源：http://hqa.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://pjn.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://qny.gaohongyu789.top

[R63] 内存与进程
来源：http://hen.ivvv.top

free -h;  ps aux | grep nginx
来源：http://kle.fanxiaobao.xyz

[R64] 结束进程
来源：http://tae.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://mnq.ybcxt.top

[R65] 查看端口占用
来源：http://qby.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ncn.ybcxt.top

[R66] 定时任务
来源：http://nab.yongpay.top

crontab -e;  crontab -l
来源：http://klv.shuidangran.top

[R67] 生成随机十六进制串
来源：http://vqs.hcnkem.com

openssl rand -hex 16
来源：http://ihg.sjlbkw.cn

[R68] 计算文件校验值
来源：http://qaf.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://yco.quarkkingdee.top

[R69] 生成随机密码
来源：http://dif.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://ymt.tanke756.top

[R70] 时间戳与互转
来源：http://jxp.xinyue.icu

date +%s;  date -d @1700000000
来源：http://nqj.vehdjk.com

[R71] 日期格式化
来源：http://jhp.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tsf.hysaishi.cn

[R72] 等待端口就绪
来源：http://oio.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://woc.zhiwuduotai.top

[R73] 分割大日志
来源：http://ezs.yongpay.top

split -l 1000 big.log part_
来源：http://xsk.uphjek.com

[R74] 批量重命名
来源：http://wjs.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vwv.tianlin.xyz

[R75] 导出环境变量
来源：http://arf.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://dyo.jinqigufen.top

[R76] 使用临时文件
来源：http://ktu.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uya.52xcode.cn

[R77] 读取用户输入
来源：http://dua.ydjk.org.cn

read -rp "请输入: " ans
来源：http://syu.cucudq.cn

[R78] 交互式菜单
来源：http://pnv.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://wna.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://ffb.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nmg.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://fyh.cashguo.top

time ./run.sh
来源：http://imc.gogol.net.cn

================================================================================
来源：http://mvm.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://rnn.wangdashe.top

================================================================================
来源：http://jzg.52xcode.cn

[S01] C：Hello World
来源：http://mev.shangyingyoupin.top

#include <stdio.h>
来源：http://cot.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tyf.hcnkem.com

[S02] C：变量与格式化输出
来源：http://dyy.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://gsn.vqdsnc.cn

[S03] C：读入整数
来源：http://vec.nanxinkj.top

int x; scanf("%d", &x);
来源：http://oxs.hnxiangtu.top

[S04] C：字符串复制
来源：http://joa.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://cff.dashuyun.cn

[S05] C：字符串长度
来源：http://ldk.quarkkingdee.top

strlen(s)
来源：http://xnz.jianghu66.top

[S06] C：字符串比较
来源：http://bco.daxiang520.top

strcmp(a, b) == 0
来源：http://kqh.sysykeji.top

[S07] C：数组遍历求和
来源：http://jqh.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nhp.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://mbg.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vrk.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://lhx.wangdashe.top


<!-- 参考信息 -->