代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://xzl.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://ivm.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://joy.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://ket.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://ngp.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pyo.smart0.xyz

[Q43] 标量子查询
来源：http://qeb.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mxo.sjlbkw.cn

[Q44] IN 子查询
来源：http://mwn.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kun.hongshengwenyu.top

[Q45] EXISTS 判断存在
来源：http://nez.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wtu.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://kzu.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://naj.ehwqpu.com

[Q47] 与平均值比较
来源：http://uxx.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://foz.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://tma.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gpm.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://kxz.gotoacloud.top

[Q49] 更新单行
来源：http://rhy.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wyi.tianlin.xyz

[Q50] 批量更新
来源：http://wep.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uns.yuxming.cn

[Q51] 用子查询更新
来源：http://paq.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://stf.gogol.net.cn

[Q52] 删除指定行
来源：http://rkg.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://bpu.ehwqpu.com

[Q53] 按条件删除
来源：http://qua.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qug.cqqwz.cn

[Q54] 清空表
来源：http://kom.cashguo.top

TRUNCATE TABLE logs;
来源：http://zes.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://kko.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aja.hammf.cn

[Q56] 密集排名（并列不占位）
来源：http://eot.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lbs.nanxuanxn.top

[Q57] 行号
来源：http://ptc.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hds.yj202588.top

[Q58] 累计求和
来源：http://cao.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngf.yangfankeji.com

[Q59] 分组内累计
来源：http://vzx.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://brj.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://evx.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eiw.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wou.jlsjyb.cn

[Q61] 移动平均
来源：http://udv.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hai.ybcxt.top

[Q62] 分组占比
来源：http://nwy.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fpy.fengsongda.top

[Q63] 开启事务
来源：http://mhm.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ghg.yj202588.top

[Q64] 提交事务
来源：http://zgu.bbcook.cn

COMMIT;
来源：http://wkc.cheryme.top

[Q65] 回滚事务
来源：http://ljk.yj20258.top

ROLLBACK;
来源：http://qap.yangfankeji.com

[Q66] 行锁查询
来源：http://foh.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yct.tarul.cn

[Q67] 设置隔离级别
来源：http://jpi.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bva.havefunace.top

[Q68] 保存点
来源：http://xuu.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://atg.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://maj.ydzc1.top

[Q69] 查看执行计划
来源：http://ptc.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vec.hnqzz.top

[Q70] 更新统计信息
来源：http://lnq.52xcode.cn

ANALYZE TABLE users;
来源：http://bai.iojbl.cn

[Q71] 查看建表语句
来源：http://okg.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://swl.zycfv.cn

[Q72] 查看索引
来源：http://fjv.jyoumei.cn

SHOW INDEX FROM users;
来源：http://gzt.jlsjyb.cn

[Q73] 查看表状态
来源：http://tkv.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nid.haohaochexian.top

[Q74] 强制使用索引
来源：http://aih.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://evg.yfazqb.com

[Q75] 日期格式化
来源：http://yat.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kzu.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://svl.feifeiyinyue.top

[Q76] 按天统计
来源：http://ege.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kiu.vehdjk.com

[Q77] 时间加减
来源：http://erk.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ysi.gotoacloud.top

[Q78] 当前时间
来源：http://ppe.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cbv.daria6918.cn

[Q79] 字符串拼接
来源：http://dlc.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zmo.cucudq.cn

[Q80] 字符串截取
来源：http://frb.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jvq.zhoulong.xyz

[Q81] 字符串替换
来源：http://ago.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qtn.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://ehw.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://law.cdnleiting.top

[Q83] 大小写转换
来源：http://ets.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kcb.zdbjq.cn

[Q84] 去除首尾空格
来源：http://hek.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://emz.birdmap.top

[Q85] 数值取整
来源：http://mse.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xkt.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://dbc.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bfx.hcnkem.com

[Q87] JSON 字段做条件
来源：http://skm.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dhf.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://pfq.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ibm.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vxl.dianchejie.cn

[Q89] 判断表是否存在
来源：http://kcs.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://inq.hammf.cn

[Q90] 生成序号列
来源：http://vid.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lwu.jianghu66.top

================================================================================
来源：http://amd.vqdsnc.cn

R. Bash 专题
来源：http://uge.zhixingplan.top

================================================================================
来源：http://zwu.cqqwz.cn

[R01] shebang 与严格模式
来源：http://qes.shzxlz.cn

#!/usr/bin/env bash
来源：http://ksv.haohaochexian.top

set -euo pipefail
来源：http://qyp.redwolf501.top

[R02] 变量赋值与使用
来源：http://asz.sweek.top

name="Tom"; echo "$name"
来源：http://muw.jqgfzy.top

[R03] 只读变量
来源：http://icr.daria6918.cn

readonly PI=3.14
来源：http://mdh.zhixingplan.top

[R04] 位置参数
来源：http://fhd.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lpr.shzxlz.cn

[R05] 参数默认值
来源：http://iwy.zhoulong.xyz

name="${1:-default}"
来源：http://btf.tarul.cn

[R06] 判断命令是否存在
来源：http://hjo.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fom.fktsv.cn

[R07] if 判断文件
来源：http://evh.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rnf.feifeiyinyue.top

[R08] 数值比较
来源：http://ddq.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gaj.vehdjk.com

[R09] 字符串比较
来源：http://wmp.guannengcc.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ljc.zhengqikj.top

[R10] 正则匹配
来源：http://ghn.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rqn.bbcook.cn

[R11] case 多分支
来源：http://kbo.wangshuangyany.cn

case "$1" in
来源：http://kcm.meibo888.top

start) echo "启动" ;;
来源：http://atv.bjfxy.top

stop)  echo "停止" ;;
来源：http://vto.meibo888.top

*)     echo "未知命令" ;;
来源：http://gda.yj202588.top

esac
来源：http://dxa.sufxvd.cn

[R12] for 遍历文件
来源：http://sch.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://rey.gotoacloud.top

[R13] for 计数循环
来源：http://nxe.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://xis.ehwqpu.com

[R14] C 风格 for
来源：http://hzn.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xdg.sysykeji.top

[R15] while 逐行读文件
来源：http://yay.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://njd.zhiwuduotai.top

[R16] until 等待条件
来源：http://tpr.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aby.sjlbkw.cn

[R17] 数组定义与取值
来源：http://jnn.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zrg.feifeiyinyue.top

[R18] 遍历数组
来源：http://paa.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lmm.zdqjudy.top

[R19] 数组长度
来源：http://fgo.redwolf501.top

echo "${#arr[@]}"
来源：http://dwa.jqgfzy.top

[R20] 关联数组（字典）
来源：http://wfp.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kxv.guowangkeji.top

[R21] 字符串长度
来源：http://sei.zhongyouzk.top

echo "${#s}"
来源：http://ksj.ehwqpu.com

[R22] 截取子串
来源：http://vmq.sxryk.cn

echo "${s:0:5}"
来源：http://iqb.gotoacloud.top

[R23] 字符串替换
来源：http://vgq.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ssg.meibo888.top

[R24] 大小写转换
来源：http://edx.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://crh.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://kvc.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pdi.hammf.cn

[R26] 命令替换
来源：http://ilj.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://nyx.birdmap.top

[R27] 算术展开
来源：http://lcn.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://acg.9152youxi.cn

[R28] 浮点运算
来源：http://uoh.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://pti.hysaishi.cn

[R29] 定义函数
来源：http://gai.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uam.svipenyu.cn

[R30] 函数返回状态码
来源：http://rsy.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://tml.yangfankeji.com

[R31] 局部变量
来源：http://ruh.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://qjv.ehwqpu.com

[R32] 参数个数校验
来源：http://dpa.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pzp.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://twp.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hbv.dashuyun.cn

[R34] 退出时清理
来源：http://qyf.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://qtt.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://acc.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zsx.mhx1999.top

[R36] 并发执行多个任务
来源：http://ajk.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rhn.sweek.top

[R37] 把输出赋给变量
来源：http://sni.jinyuanbaomall.cn

files=$(ls -1)
来源：http://jdz.c1oappe.top

[R38] 管道串联
来源：http://nrp.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://pvj.316326.xyz

[R39] 重定向标准输出与错误
来源：http://ypg.fktsv.cn

cmd > out.log 2>&1
来源：http://xbp.havefunace.top

[R40] 追加写日志
来源：http://peu.dashuyun.cn

echo "log" >> out.log
来源：http://rzj.9152youxi.cn

[R41] 丢弃输出
来源：http://doy.gzhubu.top

cmd >/dev/null 2>&1
来源：http://zwp.haohaochexian.top

[R42] 输入重定向
来源：http://jnr.jinqigufen.top

wc -l < a.txt
来源：http://xqo.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://ozp.sysykeji.top

find . -name "*.log" -type f
来源：http://hgp.jianghu66.top

[R44] 按修改时间查找
来源：http://fsg.yj20258.top

find . -mtime -7 -type f
来源：http://pnv.vqdsnc.cn

[R45] 批量删除
来源：http://jms.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://mal.guowangkeji.top

[R46] 递归替换文件内容
来源：http://jyh.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://erm.ydjk.org.cn

[R47] sed 单行替换
来源：http://ksl.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://hzw.sxryk.cn

[R48] awk 取指定列
来源：http://etk.ydzc1.top

awk '{print $1, $3}' a.txt
来源：http://vvn.c1oappe.top

[R49] awk 带条件
来源：http://hep.ppjwa.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ovb.yuxming.cn

[R50] awk 求和
来源：http://yiz.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://txk.fzhhl.top

[R51] 排序去重取前几
来源：http://dgc.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jal.cdnleiting.top

[R52] 统计行数
来源：http://zev.9152youxi.cn

wc -l a.txt
来源：http://zuc.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://usd.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xhw.cqqwz.cn

[R54] 比较两个文件
来源：http://jph.feifeiyinyue.top

diff a.txt b.txt
来源：http://lor.yj202588.top

[R55] 压缩与解压
来源：http://eqq.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rev.hammf.cn

[R56] 远程拷贝
来源：http://xjp.jinghuilouyu.cn

scp file user@host:/path/
来源：http://dej.iojbl.cn

[R57] 远程执行命令
来源：http://nan.dashuyun.cn

ssh user@host 'uptime'
来源：http://oxe.sufxvd.cn

[R58] 下载文件
来源：http://kva.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://otr.fengsongda.top

[R59] 发 POST JSON
来源：http://sgn.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vga.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://wna.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zvx.xuetiantiany.cn

[R61] 磁盘占用
来源：http://lmo.shanyushiyangtech.top

df -h;  du -sh *
来源：http://rzn.hammf.cn

[R62] 找最占空间的文件
来源：http://xqa.ivvv.top

du -ah . | sort -rh | head -10
来源：http://fzq.cdnleiting.top

[R63] 内存与进程
来源：http://mko.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://mep.9152youxi.cn

[R64] 结束进程
来源：http://sjq.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://cqw.gaohongyu789.top

[R65] 查看端口占用
来源：http://fzw.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ugc.gotoacloud.top

[R66] 定时任务
来源：http://iwe.tianlin.xyz

crontab -e;  crontab -l
来源：http://znp.sweek.top

[R67] 生成随机十六进制串
来源：http://bdg.yongpay.top

openssl rand -hex 16
来源：http://sit.316326.xyz

[R68] 计算文件校验值
来源：http://yqs.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://hgl.zhoulong.xyz

[R69] 生成随机密码
来源：http://hru.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://vfy.fktsv.cn

[R70] 时间戳与互转
来源：http://sdf.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://nbm.hnqzz.top

[R71] 日期格式化
来源：http://zrp.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qft.cheryme.top

[R72] 等待端口就绪
来源：http://bpq.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://les.nanxinkj.top

[R73] 分割大日志
来源：http://afw.mhx1999.top

split -l 1000 big.log part_
来源：http://sku.tianlin.xyz

[R74] 批量重命名
来源：http://jjx.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uxu.9152youxi.cn

[R75] 导出环境变量
来源：http://aka.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://pqb.ivvv.top

[R76] 使用临时文件
来源：http://ceh.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qkj.jqgufenzy.top

[R77] 读取用户输入
来源：http://ees.smart0.xyz

read -rp "请输入: " ans
来源：http://tpk.yj20258888.top

[R78] 交互式菜单
来源：http://kpm.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mou.uphjek.com

[R79] 解析命令行选项
来源：http://hmk.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iks.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://sww.yongpay.top

time ./run.sh
来源：http://gpf.hnqzz.top

================================================================================
来源：http://wqr.jinghuilouyu.cn

S. C / C++ 专题
来源：http://rqo.bbcook.cn

================================================================================
来源：http://txn.andypj.xyz

[S01] C：Hello World
来源：http://fha.yonumen.top

#include <stdio.h>
来源：http://gxc.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vst.epnwcf.com

[S02] C：变量与格式化输出
来源：http://ozl.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://quj.gzhubu.top

[S03] C：读入整数
来源：http://ebc.cqqwz.cn

int x; scanf("%d", &x);
来源：http://gpr.cucudq.cn

[S04] C：字符串复制
来源：http://efu.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wcc.0kj1m.cn

[S05] C：字符串长度
来源：http://sif.yuanzhike.top

strlen(s)
来源：http://iuh.yuxming.cn

[S06] C：字符串比较
来源：http://jry.jyoumei.cn

strcmp(a, b) == 0
来源：http://hur.yonumen.top

[S07] C：数组遍历求和
来源：http://gbo.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xdz.meibo888.top

[S08] C：动态内存分配与释放
来源：http://qha.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://seo.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://cfp.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rtj.nanxinkj.top

[S10] C：指针与解引用
来源：http://adx.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://ptb.jianghu66.top

[S11] C：逐行读文件
来源：http://udi.feifeiyinyue.top


<!-- 参考信息 -->