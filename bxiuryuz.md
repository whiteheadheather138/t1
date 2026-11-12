代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://tuv.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://ous.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://inr.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://wcn.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://nsq.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nja.andypj.xyz

[Q43] 标量子查询
来源：http://wsu.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mpa.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://lfw.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ucc.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://wab.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kza.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://rya.nanxinkj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdp.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://wjl.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qkn.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://wto.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lrp.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://plx.meibo888.top

[Q49] 更新单行
来源：http://ttt.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wux.tianlin.xyz

[Q50] 批量更新
来源：http://fun.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pak.andypj.xyz

[Q51] 用子查询更新
来源：http://pme.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://axj.yj202588.top

[Q52] 删除指定行
来源：http://xnu.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://rmw.redwolf501.top

[Q53] 按条件删除
来源：http://djl.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cdn.yj20258888.top

[Q54] 清空表
来源：http://jmy.guannengcc.top

TRUNCATE TABLE logs;
来源：http://rzl.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://kwv.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vce.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://tiy.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pzf.zdqjudy.top

[Q57] 行号
来源：http://dsp.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wjb.meibo888.top

[Q58] 累计求和
来源：http://ahd.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fqo.ctjpmb.com

[Q59] 分组内累计
来源：http://rfw.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gfe.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://dpp.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zph.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpp.haohaochexian.top

[Q61] 移动平均
来源：http://fjf.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xgk.sxryk.cn

[Q62] 分组占比
来源：http://evj.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ewh.redwolf501.top

[Q63] 开启事务
来源：http://wjj.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eym.hnqzz.top

[Q64] 提交事务
来源：http://nog.fktsv.cn

COMMIT;
来源：http://efy.fehbvm.com

[Q65] 回滚事务
来源：http://yvj.zhengqikj.top

ROLLBACK;
来源：http://vlg.9152youxi.cn

[Q66] 行锁查询
来源：http://ops.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qoy.tianlin.xyz

[Q67] 设置隔离级别
来源：http://qug.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vng.hnqzz.top

[Q68] 保存点
来源：http://iwx.xuanzx.com

SAVEPOINT sp1;
来源：http://epz.jianghu66.top

ROLLBACK TO sp1;
来源：http://hqh.fehbvm.com

[Q69] 查看执行计划
来源：http://ykv.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://icx.yongpay.top

[Q70] 更新统计信息
来源：http://kfo.daria6918.cn

ANALYZE TABLE users;
来源：http://pih.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://zzr.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ncb.gaohongyu789.top

[Q72] 查看索引
来源：http://cto.ybcxt.top

SHOW INDEX FROM users;
来源：http://xin.gogol.net.cn

[Q73] 查看表状态
来源：http://qvq.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uly.yanxiufei.cn

[Q74] 强制使用索引
来源：http://njw.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oob.fzhhl.top

[Q75] 日期格式化
来源：http://qqv.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fug.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zeh.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://ytq.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nwp.9152youxi.cn

[Q77] 时间加减
来源：http://pvg.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ggf.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://kpv.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cqv.fktsv.cn

[Q79] 字符串拼接
来源：http://cie.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ccq.chenlongwang.top

[Q80] 字符串截取
来源：http://utd.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ufl.smart0.xyz

[Q81] 字符串替换
来源：http://kbh.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lkm.birdmap.top

[Q82] 字符长度与字节长度
来源：http://bwt.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://upy.jqgfzy.top

[Q83] 大小写转换
来源：http://uxk.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vef.havefunace.top

[Q84] 去除首尾空格
来源：http://wlj.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://cvr.ybcxt.top

[Q85] 数值取整
来源：http://jdw.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://feb.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://kkc.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cwm.yvedp.cn

[Q87] JSON 字段做条件
来源：http://uun.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://swx.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://ryu.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eel.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kry.yuanzhike.top

[Q89] 判断表是否存在
来源：http://cqm.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gez.yj202588.top

[Q90] 生成序号列
来源：http://qgr.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hvs.ydjk.org.cn

================================================================================
来源：http://hrk.9152youxi.cn

R. Bash 专题
来源：http://vya.yongpay.top

================================================================================
来源：http://aqu.ivvv.top

[R01] shebang 与严格模式
来源：http://lwu.andypj.xyz

#!/usr/bin/env bash
来源：http://aoo.sysykeji.top

set -euo pipefail
来源：http://vwo.yueranfly.top

[R02] 变量赋值与使用
来源：http://mca.wangdashe.top

name="Tom"; echo "$name"
来源：http://trf.jianghu66.top

[R03] 只读变量
来源：http://exi.chenlongwang.top

readonly PI=3.14
来源：http://xfv.dianchejie.cn

[R04] 位置参数
来源：http://rkq.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://isg.jianghu66.top

[R05] 参数默认值
来源：http://wsw.yj20258.top

name="${1:-default}"
来源：http://tat.zhixingplan.top

[R06] 判断命令是否存在
来源：http://mdr.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qjt.zdqjudy.top

[R07] if 判断文件
来源：http://hio.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kbu.wangshuangyany.cn

[R08] 数值比较
来源：http://axt.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jmu.nanxuanxn.top

[R09] 字符串比较
来源：http://gtq.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vmq.uphjek.com

[R10] 正则匹配
来源：http://fkw.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eks.zycfv.cn

[R11] case 多分支
来源：http://xsf.yuanzhike.top

case "$1" in
来源：http://lly.shangyingyoupin.top

start) echo "启动" ;;
来源：http://gbm.xziqi.cn

stop)  echo "停止" ;;
来源：http://kzk.ydzc1.top

*)     echo "未知命令" ;;
来源：http://szb.mhx1999.top

esac
来源：http://rdg.shangyingyoupin.top

[R12] for 遍历文件
来源：http://hpa.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://hdw.hfpthk.cn

[R13] for 计数循环
来源：http://fin.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://kgv.gogol.net.cn

[R14] C 风格 for
来源：http://ydy.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mzn.yfazqb.com

[R15] while 逐行读文件
来源：http://tfr.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kpz.jiagoushi.top

[R16] until 等待条件
来源：http://blu.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ipt.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://bnw.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kjz.gogol.net.cn

[R18] 遍历数组
来源：http://xhw.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ksf.guannengcc.top

[R19] 数组长度
来源：http://mve.nwbrower.top

echo "${#arr[@]}"
来源：http://vif.yonumen.top

[R20] 关联数组（字典）
来源：http://cnq.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wyu.daria6918.cn

[R21] 字符串长度
来源：http://nsa.ybcxt.top

echo "${#s}"
来源：http://vfg.zdbjq.cn

[R22] 截取子串
来源：http://rsa.sweek.top

echo "${s:0:5}"
来源：http://vfj.dianchejie.cn

[R23] 字符串替换
来源：http://ksu.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://brn.gzhubu.top

[R24] 大小写转换
来源：http://bbg.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uye.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://stw.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ixn.dashuyun.cn

[R26] 命令替换
来源：http://jvz.tarul.cn

now=$(date +%F); echo "$now"
来源：http://squ.yonumen.top

[R27] 算术展开
来源：http://klv.guannengcc.top

echo $((1 + 2 * 3))
来源：http://rwq.hongshengwenyu.top

[R28] 浮点运算
来源：http://ojl.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://ldh.shangyingyoupin.top

[R29] 定义函数
来源：http://lrd.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jml.sysykeji.top

[R30] 函数返回状态码
来源：http://qtm.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://qvx.xuanzx.com

[R31] 局部变量
来源：http://pzd.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://wgf.yuxming.cn

[R32] 参数个数校验
来源：http://jvr.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hbd.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://sdg.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cme.c1oappe.top

[R34] 退出时清理
来源：http://zpn.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://ikw.havefunace.top

[R35] 后台执行并等待
来源：http://pdj.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lzr.dianchejie.cn

[R36] 并发执行多个任务
来源：http://rdt.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gld.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://wqg.ywan-chungtsiang.top

files=$(ls -1)
来源：http://aad.xuanzx.com

[R38] 管道串联
来源：http://thi.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://izp.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://uod.hcnkem.com

cmd > out.log 2>&1
来源：http://umm.yueranfly.top

[R40] 追加写日志
来源：http://vvc.bjfxy.top

echo "log" >> out.log
来源：http://cdx.gzhubu.top

[R41] 丢弃输出
来源：http://gbx.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://pgf.hywenlv.cn

[R42] 输入重定向
来源：http://zye.hesvh.cn

wc -l < a.txt
来源：http://kjv.yuxming.cn

[R43] 按名字查找文件
来源：http://wfj.316326.xyz

find . -name "*.log" -type f
来源：http://uze.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://qai.birdmap.top

find . -mtime -7 -type f
来源：http://mqg.shanyushiyangtech.top

[R45] 批量删除
来源：http://myg.uphjek.com

find . -name "*.tmp" -delete
来源：http://jdv.tarul.cn

[R46] 递归替换文件内容
来源：http://tmt.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://opz.jianghu66.top

[R47] sed 单行替换
来源：http://hri.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://agw.yfazqb.com

[R48] awk 取指定列
来源：http://bpb.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://tei.wangdashe.top

[R49] awk 带条件
来源：http://iji.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dxq.wangdashe.top

[R50] awk 求和
来源：http://wyl.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://qaq.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://asx.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pmk.ctjpmb.com

[R52] 统计行数
来源：http://lig.cheryme.top

wc -l a.txt
来源：http://tib.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://tbh.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://der.yanxiufei.cn

[R54] 比较两个文件
来源：http://unc.yuxming.cn

diff a.txt b.txt
来源：http://cle.hfpthk.cn

[R55] 压缩与解压
来源：http://mir.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kbs.sjlbkw.cn

[R56] 远程拷贝
来源：http://ues.bbcook.cn

scp file user@host:/path/
来源：http://dqs.cdnleiting.top

[R57] 远程执行命令
来源：http://ivf.yuanzhike.top

ssh user@host 'uptime'
来源：http://htd.yj20258888.top

[R58] 下载文件
来源：http://psc.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oun.gotoacloud.top

[R59] 发 POST JSON
来源：http://vxi.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xkr.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://yqq.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://slo.birdmap.top

[R61] 磁盘占用
来源：http://wly.hcnkem.com

df -h;  du -sh *
来源：http://zex.yj20258888.top

[R62] 找最占空间的文件
来源：http://omp.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://bux.jyoumei.cn

[R63] 内存与进程
来源：http://vri.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://hrm.svipenyu.cn

[R64] 结束进程
来源：http://uro.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://tny.iojbl.cn

[R65] 查看端口占用
来源：http://eul.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qgr.tian-w.cn

[R66] 定时任务
来源：http://lze.guowangkeji.top

crontab -e;  crontab -l
来源：http://gyb.guannengcc.top

[R67] 生成随机十六进制串
来源：http://not.zhoulong.xyz

openssl rand -hex 16
来源：http://wsi.bjfxy.top

[R68] 计算文件校验值
来源：http://unk.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://uas.yongpay.top

[R69] 生成随机密码
来源：http://uap.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://ltn.zhixingplan.top

[R70] 时间戳与互转
来源：http://kzu.c1oappe.top

date +%s;  date -d @1700000000
来源：http://mvt.ppjwa.cn

[R71] 日期格式化
来源：http://oyj.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vsz.sufxvd.cn

[R72] 等待端口就绪
来源：http://dzm.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qkf.daria6918.cn

[R73] 分割大日志
来源：http://kot.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://amu.jinqigfzy.top

[R74] 批量重命名
来源：http://xva.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ajz.sweek.top

[R75] 导出环境变量
来源：http://kpz.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://zca.52xcode.cn

[R76] 使用临时文件
来源：http://biy.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tpp.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://avw.cqqwz.cn

read -rp "请输入: " ans
来源：http://iwi.yj20258.top

[R78] 交互式菜单
来源：http://arn.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://igi.xuanzx.com

[R79] 解析命令行选项
来源：http://iyw.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ery.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://pfj.yueranfly.top

time ./run.sh
来源：http://pxs.tian-w.cn

================================================================================
来源：http://tfh.c1oappe.top

S. C / C++ 专题
来源：http://ybz.zdqjudy.top

================================================================================
来源：http://amw.hnxiangtu.top

[S01] C：Hello World
来源：http://cvw.guowangkeji.top

#include <stdio.h>
来源：http://lup.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uxc.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://tfx.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://rgm.andypj.xyz

[S03] C：读入整数
来源：http://grx.fehbvm.com

int x; scanf("%d", &x);
来源：http://jtq.tianlin.xyz

[S04] C：字符串复制
来源：http://fet.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://zho.fzhhl.top

[S05] C：字符串长度
来源：http://jts.ctjpmb.com

strlen(s)
来源：http://vvl.yuxming.cn

[S06] C：字符串比较
来源：http://xco.snrcjt.cn

strcmp(a, b) == 0
来源：http://idj.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://hgh.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ciz.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://hkd.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dgr.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://ouo.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zek.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://vja.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://wvd.yongpay.top

[S11] C：逐行读文件
来源：http://msj.cheryme.top


<!-- 参考信息 -->