代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://noq.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wwt.tianlin.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wku.quarkkingdee.top

[Q41] 多表连接
来源：http://ufb.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://ata.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://bev.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://ncd.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://oom.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://tcm.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pgo.yongpay.top

[Q43] 标量子查询
来源：http://iin.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qpd.zdbjq.cn

[Q44] IN 子查询
来源：http://jwz.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://edw.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://rwk.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pcl.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gvo.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ewh.bbcook.cn

[Q47] 与平均值比较
来源：http://afm.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dyh.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://wjc.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mbq.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://jhs.smart0.xyz

[Q49] 更新单行
来源：http://leo.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xqo.svipenyu.cn

[Q50] 批量更新
来源：http://kjq.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://irh.jianghu66.top

[Q51] 用子查询更新
来源：http://oot.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://phx.nwbrower.top

[Q52] 删除指定行
来源：http://exi.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://orn.ehwqpu.com

[Q53] 按条件删除
来源：http://bov.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://poa.cashguo.top

[Q54] 清空表
来源：http://qsz.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://vfy.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://ccv.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gpj.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://gjb.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oha.meibo888.top

[Q57] 行号
来源：http://ukr.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vgu.zhoulong.xyz

[Q58] 累计求和
来源：http://jno.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gqi.sxryk.cn

[Q59] 分组内累计
来源：http://xel.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cvp.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://qtq.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://agi.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wwo.zhoulong.xyz

[Q61] 移动平均
来源：http://ife.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://atm.shzxlz.cn

[Q62] 分组占比
来源：http://kss.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xkv.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://vjn.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mjy.nanxinkj.top

[Q64] 提交事务
来源：http://gvh.yangfankeji.com

COMMIT;
来源：http://eal.jinqigfzy.top

[Q65] 回滚事务
来源：http://gij.zhiwuduotai.top

ROLLBACK;
来源：http://iro.daria6918.cn

[Q66] 行锁查询
来源：http://wnu.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://crr.meibo888.top

[Q67] 设置隔离级别
来源：http://mjg.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kmp.xylfe.cn

[Q68] 保存点
来源：http://lmw.cucudq.cn

SAVEPOINT sp1;
来源：http://rsk.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://ysi.nanxinkj.top

[Q69] 查看执行计划
来源：http://fcl.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cxh.c1oappe.top

[Q70] 更新统计信息
来源：http://dnh.hnxiangtu.top

ANALYZE TABLE users;
来源：http://jrh.yfazqb.com

[Q71] 查看建表语句
来源：http://tqf.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zay.ppjwa.cn

[Q72] 查看索引
来源：http://omv.sysykeji.top

SHOW INDEX FROM users;
来源：http://nbs.xuetiantiany.cn

[Q73] 查看表状态
来源：http://yqc.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://vst.snrcjt.cn

[Q74] 强制使用索引
来源：http://rfd.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gjp.jqgufenzy.top

[Q75] 日期格式化
来源：http://ggc.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xdu.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fnp.shanyushiyangtech.top

[Q76] 按天统计
来源：http://miz.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dry.jqgfzy.top

[Q77] 时间加减
来源：http://wmu.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qmc.aibaodan.cn

[Q78] 当前时间
来源：http://kee.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vpg.fzhhl.top

[Q79] 字符串拼接
来源：http://voy.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://llm.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://byd.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mhm.tianlin.xyz

[Q81] 字符串替换
来源：http://yql.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sxz.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://wpj.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cam.nanxinkj.top

[Q83] 大小写转换
来源：http://pmk.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nmj.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://sfd.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://wpn.sweek.top

[Q85] 数值取整
来源：http://ixt.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zke.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://iqq.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fsx.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://ojj.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yuh.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://xun.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nsy.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xha.iojbl.cn

[Q89] 判断表是否存在
来源：http://owj.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zkc.hammf.cn

[Q90] 生成序号列
来源：http://xha.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qil.hfpthk.cn

================================================================================
来源：http://bep.hesvh.cn

R. Bash 专题
来源：http://mkk.sjlbkw.cn

================================================================================
来源：http://uao.sysykeji.top

[R01] shebang 与严格模式
来源：http://mns.yj202588.top

#!/usr/bin/env bash
来源：http://lob.nanxinkj.top

set -euo pipefail
来源：http://xlk.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://aza.tarul.cn

name="Tom"; echo "$name"
来源：http://ioa.ctjpmb.com

[R03] 只读变量
来源：http://jyi.sysykeji.top

readonly PI=3.14
来源：http://gid.vehdjk.com

[R04] 位置参数
来源：http://jyp.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ayb.jiagoushi.top

[R05] 参数默认值
来源：http://ztc.hnqzz.top

name="${1:-default}"
来源：http://usy.jqgfzy.top

[R06] 判断命令是否存在
来源：http://mij.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://seh.zhiwuduotai.top

[R07] if 判断文件
来源：http://hjr.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ihk.yuanzhike.top

[R08] 数值比较
来源：http://fnx.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://alh.andypj.xyz

[R09] 字符串比较
来源：http://doa.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nsw.316326.xyz

[R10] 正则匹配
来源：http://lia.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bdz.meibo888.top

[R11] case 多分支
来源：http://kjm.sxryk.cn

case "$1" in
来源：http://mtf.dianchejie.cn

start) echo "启动" ;;
来源：http://vak.cheryme.top

stop)  echo "停止" ;;
来源：http://wua.fehbvm.com

*)     echo "未知命令" ;;
来源：http://xph.haohaochexian.top

esac
来源：http://oae.yonumen.top

[R12] for 遍历文件
来源：http://fal.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://vbq.birdmap.top

[R13] for 计数循环
来源：http://iin.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://oli.cashguo.top

[R14] C 风格 for
来源：http://fyh.fzhhl.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zws.xuanzx.com

[R15] while 逐行读文件
来源：http://kqb.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://izh.smart0.xyz

[R16] until 等待条件
来源：http://ddn.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wrb.shzxlz.cn

[R17] 数组定义与取值
来源：http://wbl.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://wux.zhixingplan.top

[R18] 遍历数组
来源：http://ebd.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jxz.chenzaomai.com

[R19] 数组长度
来源：http://cqm.chenlongwang.top

echo "${#arr[@]}"
来源：http://qrs.tarul.cn

[R20] 关联数组（字典）
来源：http://fmv.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jhh.daria6918.cn

[R21] 字符串长度
来源：http://veh.shuidangran.top

echo "${#s}"
来源：http://ems.jinyuanbaomall.cn

[R22] 截取子串
来源：http://spl.nwbrower.top

echo "${s:0:5}"
来源：http://cqv.ivvv.top

[R23] 字符串替换
来源：http://xzo.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ijm.chenjidiqi.icu

[R24] 大小写转换
来源：http://tjt.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://wtv.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://amm.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hbj.9152youxi.cn

[R26] 命令替换
来源：http://cfk.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://ybd.shanyushiyangtech.top

[R27] 算术展开
来源：http://rqd.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://uyw.ydzc1.top

[R28] 浮点运算
来源：http://uiz.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://sxo.jyoumei.cn

[R29] 定义函数
来源：http://rmt.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://osl.hysaishi.cn

[R30] 函数返回状态码
来源：http://pvr.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://lnq.ybcxt.top

[R31] 局部变量
来源：http://zxj.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://gfj.shzxlz.cn

[R32] 参数个数校验
来源：http://dng.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mbb.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://npg.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://stl.gzhubu.top

[R34] 退出时清理
来源：http://ucg.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://ide.fengsongda.top

[R35] 后台执行并等待
来源：http://asi.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xzb.hfpthk.cn

[R36] 并发执行多个任务
来源：http://yqd.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iff.316326.xyz

[R37] 把输出赋给变量
来源：http://olh.0kj1m.cn

files=$(ls -1)
来源：http://srk.yj20258888.top

[R38] 管道串联
来源：http://qqg.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://vfx.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://wqo.c1oappe.top

cmd > out.log 2>&1
来源：http://vzj.tarul.cn

[R40] 追加写日志
来源：http://pwd.ydjk.org.cn

echo "log" >> out.log
来源：http://rxn.ivvv.top

[R41] 丢弃输出
来源：http://lpa.xinyue.icu

cmd >/dev/null 2>&1
来源：http://emn.jyoumei.cn

[R42] 输入重定向
来源：http://iyp.chenjidiqi.icu

wc -l < a.txt
来源：http://irg.xinyue.icu

[R43] 按名字查找文件
来源：http://cxh.svipenyu.cn

find . -name "*.log" -type f
来源：http://vll.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://dal.uphjek.com

find . -mtime -7 -type f
来源：http://xxt.bjfxy.top

[R45] 批量删除
来源：http://gix.bjfxy.top

find . -name "*.tmp" -delete
来源：http://tbw.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://ent.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebt.pengpengdd.cyou

[R47] sed 单行替换
来源：http://vba.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jnh.hcnkem.com

[R48] awk 取指定列
来源：http://jsz.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://mxv.xuetiantiany.cn

[R49] awk 带条件
来源：http://vtj.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mpb.zhiwuduotai.top

[R50] awk 求和
来源：http://cpy.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://bio.dashuyun.cn

[R51] 排序去重取前几
来源：http://enl.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://hax.zhengqikj.top

[R52] 统计行数
来源：http://vbl.jqgufenzy.top

wc -l a.txt
来源：http://fov.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://ocf.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zoc.guannengcc.top

[R54] 比较两个文件
来源：http://vcn.0kj1m.cn

diff a.txt b.txt
来源：http://jcg.bjfxy.top

[R55] 压缩与解压
来源：http://hbf.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bky.hcnkem.com

[R56] 远程拷贝
来源：http://xrr.ppjwa.cn

scp file user@host:/path/
来源：http://wtf.hfpthk.cn

[R57] 远程执行命令
来源：http://drq.fktsv.cn

ssh user@host 'uptime'
来源：http://vuu.andypj.xyz

[R58] 下载文件
来源：http://lhu.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://foy.gzhubu.top

[R59] 发 POST JSON
来源：http://dxp.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kti.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://nia.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ues.52xcode.cn

[R61] 磁盘占用
来源：http://rec.0kj1m.cn

df -h;  du -sh *
来源：http://tav.yuxming.cn

[R62] 找最占空间的文件
来源：http://zmv.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://awi.ivvv.top

[R63] 内存与进程
来源：http://hdz.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://ara.gzhubu.top

[R64] 结束进程
来源：http://pvn.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://kmy.cdnleiting.top

[R65] 查看端口占用
来源：http://msu.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qxc.uphjek.com

[R66] 定时任务
来源：http://ifk.cashguo.top

crontab -e;  crontab -l
来源：http://bdy.fktsv.cn

[R67] 生成随机十六进制串
来源：http://mfs.dashuyun.cn

openssl rand -hex 16
来源：http://cwy.yj20258.top

[R68] 计算文件校验值
来源：http://gde.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://sqo.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://lba.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://qcx.xziqi.cn

[R70] 时间戳与互转
来源：http://etc.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://vto.yvedp.cn

[R71] 日期格式化
来源：http://eey.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpo.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://axx.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://srb.pengpengdd.cyou

[R73] 分割大日志
来源：http://urh.nwbrower.top

split -l 1000 big.log part_
来源：http://mvy.snrcjt.cn

[R74] 批量重命名
来源：http://min.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ajw.sweek.top

[R75] 导出环境变量
来源：http://yqs.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://mfj.chenzaomai.com

[R76] 使用临时文件
来源：http://pas.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lgy.zdbjq.cn

[R77] 读取用户输入
来源：http://twh.andypj.xyz

read -rp "请输入: " ans
来源：http://jpj.hysaishi.cn

[R78] 交互式菜单
来源：http://zlp.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fwd.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://jww.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pli.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://rgs.snrcjt.cn

time ./run.sh
来源：http://opm.yangfankeji.com

================================================================================
来源：http://kfs.yueranfly.top

S. C / C++ 专题
来源：http://nbu.andypj.xyz

================================================================================
来源：http://iyd.chenlongwang.top

[S01] C：Hello World
来源：http://kyg.hysaishi.cn

#include <stdio.h>
来源：http://jyk.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://chc.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://xbz.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://khj.yonumen.top

[S03] C：读入整数
来源：http://wlq.xuanzx.com

int x; scanf("%d", &x);
来源：http://uqd.yvedp.cn

[S04] C：字符串复制
来源：http://etr.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zxa.yanxiufei.cn

[S05] C：字符串长度
来源：http://frc.daria6918.cn

strlen(s)
来源：http://uyf.dianchejie.cn

[S06] C：字符串比较
来源：http://nnb.bbcook.cn

strcmp(a, b) == 0
来源：http://ycy.birdmap.top

[S07] C：数组遍历求和
来源：http://lgd.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ddx.meibo888.top

[S08] C：动态内存分配与释放
来源：http://gll.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gqm.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://eee.ivvv.top


<!-- 参考信息 -->