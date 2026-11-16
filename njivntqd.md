代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nal.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sql.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tsa.ppjwa.cn

[Q41] 多表连接
来源：http://xqi.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wbb.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://nak.tian-w.cn

JOIN products p ON p.id = o.product_id;
来源：http://met.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://mam.bbcook.cn

SELECT u.name, o.amount FROM users u
来源：http://dpz.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://whw.shangyingyoupin.top

[Q43] 标量子查询
来源：http://oew.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sqy.uphjek.com

[Q44] IN 子查询
来源：http://doj.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nmr.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://any.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rop.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dfj.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kez.yj20258888.top

[Q47] 与平均值比较
来源：http://urs.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xfs.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://wvi.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://njc.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://efh.zdqjudy.top

[Q49] 更新单行
来源：http://aml.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oug.hongshengwenyu.top

[Q50] 批量更新
来源：http://pmy.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ubo.fengsongda.top

[Q51] 用子查询更新
来源：http://osy.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zbu.ppjwa.cn

[Q52] 删除指定行
来源：http://lhp.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://cos.cqqwz.cn

[Q53] 按条件删除
来源：http://tpv.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lyj.zhengqikj.top

[Q54] 清空表
来源：http://rxs.guannengcc.top

TRUNCATE TABLE logs;
来源：http://mky.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://wuk.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://okf.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://alz.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddl.jyoumei.cn

[Q57] 行号
来源：http://mti.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fuj.chenlongwang.top

[Q58] 累计求和
来源：http://mmx.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://buz.wangdashe.top

[Q59] 分组内累计
来源：http://dre.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xer.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://cvy.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mvp.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oyi.mhx1999.top

[Q61] 移动平均
来源：http://cvp.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dkn.fzhhl.top

[Q62] 分组占比
来源：http://jfg.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aou.ydjk.org.cn

[Q63] 开启事务
来源：http://qme.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cyw.wangdashe.top

[Q64] 提交事务
来源：http://gbv.hfpthk.cn

COMMIT;
来源：http://yte.pengpengdd.cyou

[Q65] 回滚事务
来源：http://ito.hnqzz.top

ROLLBACK;
来源：http://vck.tarul.cn

[Q66] 行锁查询
来源：http://kha.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fsk.zdqjudy.top

[Q67] 设置隔离级别
来源：http://omp.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cwn.bjfxy.top

[Q68] 保存点
来源：http://viv.wangdashe.top

SAVEPOINT sp1;
来源：http://lif.cucudq.cn

ROLLBACK TO sp1;
来源：http://lhq.9152youxi.cn

[Q69] 查看执行计划
来源：http://ejy.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mah.yj202588.top

[Q70] 更新统计信息
来源：http://sfz.c1oappe.top

ANALYZE TABLE users;
来源：http://aqk.zdqjudy.top

[Q71] 查看建表语句
来源：http://gta.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://djp.cashguo.top

[Q72] 查看索引
来源：http://wgh.tian-w.cn

SHOW INDEX FROM users;
来源：http://gce.svipenyu.cn

[Q73] 查看表状态
来源：http://gtx.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://wdv.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://teh.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cbe.meibo888.top

[Q75] 日期格式化
来源：http://hul.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fbh.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qfg.zhongyouzk.top

[Q76] 按天统计
来源：http://wrp.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dgb.dianchejie.cn

[Q77] 时间加减
来源：http://nwo.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eyl.bbcook.cn

[Q78] 当前时间
来源：http://vhg.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zuj.andypj.xyz

[Q79] 字符串拼接
来源：http://xkr.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yza.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://kjs.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vkm.jinqigfzy.top

[Q81] 字符串替换
来源：http://uii.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ozn.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://hek.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bbw.nanxuanxn.top

[Q83] 大小写转换
来源：http://nur.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bam.fktsv.cn

[Q84] 去除首尾空格
来源：http://fuz.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://gdf.cashguo.top

[Q85] 数值取整
来源：http://hsh.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fkg.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://bia.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mvj.snrcjt.cn

[Q87] JSON 字段做条件
来源：http://uos.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vtd.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://dyo.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fih.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sxt.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://wso.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zbz.chenzaomai.com

[Q90] 生成序号列
来源：http://wwr.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fii.yanxiufei.cn

================================================================================
来源：http://xow.ivvv.top

R. Bash 专题
来源：http://ckv.jqgfzy.top

================================================================================
来源：http://nas.yuxming.cn

[R01] shebang 与严格模式
来源：http://ugd.iojbl.cn

#!/usr/bin/env bash
来源：http://oyx.xingfuxueyuan.xyz

set -euo pipefail
来源：http://ocm.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://eps.pycfn.com

name="Tom"; echo "$name"
来源：http://pjq.hnxiangtu.top

[R03] 只读变量
来源：http://ygl.nwbrower.top

readonly PI=3.14
来源：http://qsp.tarul.cn

[R04] 位置参数
来源：http://ajp.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://txg.yuanzhike.top

[R05] 参数默认值
来源：http://sfe.fanxiaobao.xyz

name="${1:-default}"
来源：http://jyj.zhengqikj.top

[R06] 判断命令是否存在
来源：http://spm.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nlw.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://lvp.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ldu.bjfxy.top

[R08] 数值比较
来源：http://qyv.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bqe.sweek.top

[R09] 字符串比较
来源：http://svk.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iqh.gaohongyu789.top

[R10] 正则匹配
来源：http://npu.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kti.zhiwuduotai.top

[R11] case 多分支
来源：http://kgs.jqgfzy.top

case "$1" in
来源：http://gai.jlsjyb.cn

start) echo "启动" ;;
来源：http://ccx.zhixingplan.top

stop)  echo "停止" ;;
来源：http://oyl.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://gyl.jianghu66.top

esac
来源：http://tel.yanxiufei.cn

[R12] for 遍历文件
来源：http://isb.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://ret.aibaodan.cn

[R13] for 计数循环
来源：http://ewz.cucudq.cn

for i in {1..10}; do echo "$i"; done
来源：http://gra.chenjidiqi.icu

[R14] C 风格 for
来源：http://zcv.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dwq.hnxiangtu.top

[R15] while 逐行读文件
来源：http://eaj.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vfo.fehbvm.com

[R16] until 等待条件
来源：http://zjw.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jpx.fktsv.cn

[R17] 数组定义与取值
来源：http://htu.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://qdg.daria6918.cn

[R18] 遍历数组
来源：http://opj.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vuy.cashguo.top

[R19] 数组长度
来源：http://lwz.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://pvb.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://fce.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ovl.yanxiufei.cn

[R21] 字符串长度
来源：http://vjg.fengsongda.top

echo "${#s}"
来源：http://agy.tanke756.top

[R22] 截取子串
来源：http://rxb.hcnkem.com

echo "${s:0:5}"
来源：http://yey.havefunace.top

[R23] 字符串替换
来源：http://jje.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wyl.52xcode.cn

[R24] 大小写转换
来源：http://ysm.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://xjz.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://ptv.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mdo.hammf.cn

[R26] 命令替换
来源：http://ovk.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://weh.cashguo.top

[R27] 算术展开
来源：http://mmp.hcnkem.com

echo $((1 + 2 * 3))
来源：http://cge.redwolf501.top

[R28] 浮点运算
来源：http://kws.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://qqo.zdqjudy.top

[R29] 定义函数
来源：http://ldp.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qgk.zdbjq.cn

[R30] 函数返回状态码
来源：http://wrg.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://ecg.feifeiyinyue.top

[R31] 局部变量
来源：http://vlo.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://lft.xuetiantiany.cn

[R32] 参数个数校验
来源：http://hfw.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nkd.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://yyo.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://czo.ppjwa.cn

[R34] 退出时清理
来源：http://nzd.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://drj.gzhubu.top

[R35] 后台执行并等待
来源：http://zgj.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fuj.hesvh.cn

[R36] 并发执行多个任务
来源：http://ktj.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eln.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://yom.fktsv.cn

files=$(ls -1)
来源：http://ehy.daria6918.cn

[R38] 管道串联
来源：http://xuy.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://uws.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://jxh.kuanghao11.cn

cmd > out.log 2>&1
来源：http://ivp.daria6918.cn

[R40] 追加写日志
来源：http://fuf.shzxlz.cn

echo "log" >> out.log
来源：http://wrx.wangshuangyany.cn

[R41] 丢弃输出
来源：http://xfr.guannengcc.top

cmd >/dev/null 2>&1
来源：http://arv.zhongyouzk.top

[R42] 输入重定向
来源：http://kvw.meibo888.top

wc -l < a.txt
来源：http://jim.pycfn.com

[R43] 按名字查找文件
来源：http://who.birdmap.top

find . -name "*.log" -type f
来源：http://syt.xuanzx.com

[R44] 按修改时间查找
来源：http://nap.smart0.xyz

find . -mtime -7 -type f
来源：http://mfo.zhijiandao.cn

[R45] 批量删除
来源：http://njl.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://fhg.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://ewh.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hqd.aizwys.cn

[R47] sed 单行替换
来源：http://ujw.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://ttp.aizwys.cn

[R48] awk 取指定列
来源：http://iur.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://opf.svipenyu.cn

[R49] awk 带条件
来源：http://eca.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bco.daria6918.cn

[R50] awk 求和
来源：http://emr.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://wji.tian-w.cn

[R51] 排序去重取前几
来源：http://smb.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vkg.cashguo.top

[R52] 统计行数
来源：http://qao.sufxvd.cn

wc -l a.txt
来源：http://ete.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://ekp.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zsy.yuanzhike.top

[R54] 比较两个文件
来源：http://pzf.0kj1m.cn

diff a.txt b.txt
来源：http://hsx.cashguo.top

[R55] 压缩与解压
来源：http://pgy.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vly.0kj1m.cn

[R56] 远程拷贝
来源：http://wvh.fehbvm.com

scp file user@host:/path/
来源：http://fhq.zycfv.cn

[R57] 远程执行命令
来源：http://mlb.aizwys.cn

ssh user@host 'uptime'
来源：http://iij.svipenyu.cn

[R58] 下载文件
来源：http://abn.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wyg.aizwys.cn

[R59] 发 POST JSON
来源：http://ixy.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lpu.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://jnm.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xwn.0kj1m.cn

[R61] 磁盘占用
来源：http://ftf.yonumen.top

df -h;  du -sh *
来源：http://wmt.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://jla.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://iuh.birdmap.top

[R63] 内存与进程
来源：http://jqq.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://del.zhengqikj.top

[R64] 结束进程
来源：http://rcx.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://fiy.dashuyun.cn

[R65] 查看端口占用
来源：http://pyz.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ofl.epnwcf.com

[R66] 定时任务
来源：http://gaa.shuidangran.top

crontab -e;  crontab -l
来源：http://jip.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://hka.yj20258.top

openssl rand -hex 16
来源：http://vsx.yj20258.top

[R68] 计算文件校验值
来源：http://nbc.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://ecx.jqgufenzy.top

[R69] 生成随机密码
来源：http://mmk.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://mjd.meibo888.top

[R70] 时间戳与互转
来源：http://wku.yuxming.cn

date +%s;  date -d @1700000000
来源：http://nkk.tian-w.cn

[R71] 日期格式化
来源：http://mmz.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cmr.jianghu66.top

[R72] 等待端口就绪
来源：http://gzb.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ieu.9152youxi.cn

[R73] 分割大日志
来源：http://lbc.yfazqb.com

split -l 1000 big.log part_
来源：http://pin.c1oappe.top

[R74] 批量重命名
来源：http://ljh.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jph.yangfankeji.com

[R75] 导出环境变量
来源：http://lms.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://joo.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://dpp.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ziu.chenjidiqi.icu

[R77] 读取用户输入
来源：http://ccf.gaohongyu789.top

read -rp "请输入: " ans
来源：http://udi.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://ekt.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tip.nanxinkj.top

[R79] 解析命令行选项
来源：http://kmk.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hir.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://glz.daxiang520.top

time ./run.sh
来源：http://pyy.hywenlv.cn

================================================================================
来源：http://mzt.zhiwuduotai.top

S. C / C++ 专题
来源：http://vtl.fzhhl.top

================================================================================
来源：http://ifp.tianlin.xyz

[S01] C：Hello World
来源：http://pjn.jianghu66.top

#include <stdio.h>
来源：http://idv.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vua.sxryk.cn

[S02] C：变量与格式化输出
来源：http://cvt.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://fau.pycfn.com

[S03] C：读入整数
来源：http://mda.hywenlv.cn

int x; scanf("%d", &x);
来源：http://vku.gotoacloud.top

[S04] C：字符串复制
来源：http://kgt.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://aqs.hywenlv.cn

[S05] C：字符串长度
来源：http://wui.xingfuxueyuan.xyz

strlen(s)
来源：http://gbr.xuanzx.com

[S06] C：字符串比较
来源：http://sxg.xinyue.icu

strcmp(a, b) == 0
来源：http://xsi.guowangkeji.top

[S07] C：数组遍历求和
来源：http://ekm.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gdq.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://azl.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hqn.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://jcb.hnxiangtu.top


<!-- 参考信息 -->