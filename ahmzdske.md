代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://vvy.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ehz.jqgfzy.top

[Q43] 标量子查询
来源：http://tio.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lcs.52xcode.cn

[Q44] IN 子查询
来源：http://rvw.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dep.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://nva.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uyu.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://jrj.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://des.zycfv.cn

[Q47] 与平均值比较
来源：http://kss.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gps.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://cyx.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vox.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://qto.cqqwz.cn

[Q49] 更新单行
来源：http://etu.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wbd.gogol.net.cn

[Q50] 批量更新
来源：http://wxf.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xcm.zycfv.cn

[Q51] 用子查询更新
来源：http://fxu.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ttw.yanxiufei.cn

[Q52] 删除指定行
来源：http://yky.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://mfw.daria6918.cn

[Q53] 按条件删除
来源：http://gog.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dlo.daxiang520.top

[Q54] 清空表
来源：http://emo.yj20258.top

TRUNCATE TABLE logs;
来源：http://bmf.mhx1999.top

[Q55] 排名（并列占位）
来源：http://xwx.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vol.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://xkk.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ijt.shanyushiyangkeji.top

[Q57] 行号
来源：http://txd.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xdx.iojbl.cn

[Q58] 累计求和
来源：http://ycn.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bqq.yonumen.top

[Q59] 分组内累计
来源：http://kqg.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ubn.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://pca.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fnb.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uvo.hnxiangtu.top

[Q61] 移动平均
来源：http://hfj.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kjt.meibo888.top

[Q62] 分组占比
来源：http://pfm.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hha.wangshuangyany.cn

[Q63] 开启事务
来源：http://tlo.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ypq.fanxiaobao.xyz

[Q64] 提交事务
来源：http://oqh.yonumen.top

COMMIT;
来源：http://hob.haohaochexian.top

[Q65] 回滚事务
来源：http://koc.pengpengdd.cyou

ROLLBACK;
来源：http://kzx.fktsv.cn

[Q66] 行锁查询
来源：http://yyy.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wjz.guowangkeji.top

[Q67] 设置隔离级别
来源：http://uqw.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ncf.birdmap.top

[Q68] 保存点
来源：http://clw.zdqjudy.top

SAVEPOINT sp1;
来源：http://cip.haohaochexian.top

ROLLBACK TO sp1;
来源：http://xhz.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://uky.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xoe.yfazqb.com

[Q70] 更新统计信息
来源：http://zol.nanxuanxn.top

ANALYZE TABLE users;
来源：http://wlr.yj20258.top

[Q71] 查看建表语句
来源：http://czn.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jht.svipenyu.cn

[Q72] 查看索引
来源：http://ngm.cucudq.cn

SHOW INDEX FROM users;
来源：http://kun.birdmap.top

[Q73] 查看表状态
来源：http://csg.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lci.jqgufenzy.top

[Q74] 强制使用索引
来源：http://vhy.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dnn.jlsjyb.cn

[Q75] 日期格式化
来源：http://azt.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dgj.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ugq.zdqjudy.top

[Q76] 按天统计
来源：http://xzb.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uzm.mhx1999.top

[Q77] 时间加减
来源：http://jmr.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pxe.jinqigfzy.top

[Q78] 当前时间
来源：http://oow.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hqr.svipenyu.cn

[Q79] 字符串拼接
来源：http://zws.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gvl.havefunace.top

[Q80] 字符串截取
来源：http://nov.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vze.zhiwuduotai.top

[Q81] 字符串替换
来源：http://qim.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wuy.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://dng.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jti.yj20258888.top

[Q83] 大小写转换
来源：http://aix.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://udt.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://vkb.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://kin.52xcode.cn

[Q85] 数值取整
来源：http://fvj.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zmt.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://rqn.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dfk.yuxming.cn

[Q87] JSON 字段做条件
来源：http://ave.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nuh.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://lud.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://csm.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://emy.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://vzx.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wfj.yj20258888.top

[Q90] 生成序号列
来源：http://aav.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jej.yfazqb.com

================================================================================
来源：http://vmr.hcnkem.com

R. Bash 专题
来源：http://eax.gaohongyu789.top

================================================================================
来源：http://qlf.sxryk.cn

[R01] shebang 与严格模式
来源：http://bah.shuidangran.top

#!/usr/bin/env bash
来源：http://wnj.smart0.xyz

set -euo pipefail
来源：http://xod.cdnleiting.top

[R02] 变量赋值与使用
来源：http://zfg.bjfxy.top

name="Tom"; echo "$name"
来源：http://tke.hongshengwenyu.top

[R03] 只读变量
来源：http://dlo.feifeiyinyue.top

readonly PI=3.14
来源：http://aqj.yvedp.cn

[R04] 位置参数
来源：http://lzz.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uyi.zhongyouzk.top

[R05] 参数默认值
来源：http://dnl.chenlongwang.top

name="${1:-default}"
来源：http://lsl.nanxinkj.top

[R06] 判断命令是否存在
来源：http://nmy.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kjg.zdqjudy.top

[R07] if 判断文件
来源：http://igb.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nga.chenzaomai.com

[R08] 数值比较
来源：http://yki.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wkm.zhiwuduotai.top

[R09] 字符串比较
来源：http://fyy.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sjt.zhongyouzk.top

[R10] 正则匹配
来源：http://ckw.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pda.hesvh.cn

[R11] case 多分支
来源：http://ivw.ivvv.top

case "$1" in
来源：http://iem.fzhhl.top

start) echo "启动" ;;
来源：http://rha.dashuyun.cn

stop)  echo "停止" ;;
来源：http://rus.xziqi.cn

*)     echo "未知命令" ;;
来源：http://ovz.jlsjyb.cn

esac
来源：http://vnf.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://goi.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://zrc.fktsv.cn

[R13] for 计数循环
来源：http://qhh.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://wmc.chenzaomai.com

[R14] C 风格 for
来源：http://dxd.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rco.hnxiangtu.top

[R15] while 逐行读文件
来源：http://dnk.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fpg.gotoacloud.top

[R16] until 等待条件
来源：http://ntp.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://olp.daxiang520.top

[R17] 数组定义与取值
来源：http://iux.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://toe.jlsjyb.cn

[R18] 遍历数组
来源：http://qya.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dyt.nanxuanxn.top

[R19] 数组长度
来源：http://dwz.svipenyu.cn

echo "${#arr[@]}"
来源：http://qlc.gogol.net.cn

[R20] 关联数组（字典）
来源：http://oul.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tnn.uphjek.com

[R21] 字符串长度
来源：http://icc.gogol.net.cn

echo "${#s}"
来源：http://vds.jinyuanbaomall.cn

[R22] 截取子串
来源：http://uit.yfazqb.com

echo "${s:0:5}"
来源：http://agg.hywenlv.cn

[R23] 字符串替换
来源：http://etm.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bfe.sweek.top

[R24] 大小写转换
来源：http://ime.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://pzl.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://lbu.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ixl.vqdsnc.cn

[R26] 命令替换
来源：http://pht.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://ucl.fanxiaobao.xyz

[R27] 算术展开
来源：http://emb.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://nuc.tian-w.cn

[R28] 浮点运算
来源：http://tkl.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://yps.nanxuanxn.top

[R29] 定义函数
来源：http://utd.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xkb.shzxlz.cn

[R30] 函数返回状态码
来源：http://aug.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://sqw.cdnleiting.top

[R31] 局部变量
来源：http://laz.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://zhp.ydjk.org.cn

[R32] 参数个数校验
来源：http://dpr.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pie.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://qzm.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://roa.pengpengdd.cyou

[R34] 退出时清理
来源：http://cbf.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jqu.cashguo.top

[R35] 后台执行并等待
来源：http://hmy.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wcn.jinqigufen.top

[R36] 并发执行多个任务
来源：http://szx.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wcc.svipenyu.cn

[R37] 把输出赋给变量
来源：http://lal.svipenyu.cn

files=$(ls -1)
来源：http://jhh.yfazqb.com

[R38] 管道串联
来源：http://oah.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://itg.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://dyx.xziqi.cn

cmd > out.log 2>&1
来源：http://fxm.cqqwz.cn

[R40] 追加写日志
来源：http://ity.sxryk.cn

echo "log" >> out.log
来源：http://ezf.fehbvm.com

[R41] 丢弃输出
来源：http://egf.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://wsn.epnwcf.com

[R42] 输入重定向
来源：http://iye.tian-w.cn

wc -l < a.txt
来源：http://aub.cdnleiting.top

[R43] 按名字查找文件
来源：http://vgc.jianghu66.top

find . -name "*.log" -type f
来源：http://pif.yangfankeji.com

[R44] 按修改时间查找
来源：http://keh.uphjek.com

find . -mtime -7 -type f
来源：http://byr.yongpay.top

[R45] 批量删除
来源：http://jjs.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://tpq.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://srx.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gco.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://wsk.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://wwf.nanxinkj.top

[R48] awk 取指定列
来源：http://rbj.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://rqz.jiagoushi.top

[R49] awk 带条件
来源：http://wai.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ziq.vehdjk.com

[R50] awk 求和
来源：http://tim.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lnd.zycfv.cn

[R51] 排序去重取前几
来源：http://tvu.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://nja.vqdsnc.cn

[R52] 统计行数
来源：http://qwx.jinyuanbaomall.cn

wc -l a.txt
来源：http://gfc.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://wzo.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tuq.fengsongda.top

[R54] 比较两个文件
来源：http://xkm.wangdashe.top

diff a.txt b.txt
来源：http://bxs.chenzaomai.com

[R55] 压缩与解压
来源：http://jmf.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ygo.chenjidiqi.icu

[R56] 远程拷贝
来源：http://evs.wangdashe.top

scp file user@host:/path/
来源：http://uni.fktsv.cn

[R57] 远程执行命令
来源：http://fdj.jlsjyb.cn

ssh user@host 'uptime'
来源：http://suc.chenlongwang.top

[R58] 下载文件
来源：http://crk.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vzn.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://lhw.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ang.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://pzg.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://srw.zhiwuduotai.top

[R61] 磁盘占用
来源：http://ctw.yj202588.top

df -h;  du -sh *
来源：http://tvj.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://non.uphjek.com

du -ah . | sort -rh | head -10
来源：http://zpp.mhx1999.top

[R63] 内存与进程
来源：http://xme.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://pma.vqdsnc.cn

[R64] 结束进程
来源：http://fql.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://gug.hammf.cn

[R65] 查看端口占用
来源：http://sys.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qdt.zhongyouzk.top

[R66] 定时任务
来源：http://djy.dianchejie.cn

crontab -e;  crontab -l
来源：http://xxz.xinyue.icu

[R67] 生成随机十六进制串
来源：http://ibs.guannengcc.top

openssl rand -hex 16
来源：http://neh.daxiang520.top

[R68] 计算文件校验值
来源：http://tji.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://gpa.daria6918.cn

[R69] 生成随机密码
来源：http://rup.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://ryd.xinyue.icu

[R70] 时间戳与互转
来源：http://tjt.xylfe.cn

date +%s;  date -d @1700000000
来源：http://ghu.sufxvd.cn

[R71] 日期格式化
来源：http://zpj.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jth.52xcode.cn

[R72] 等待端口就绪
来源：http://wqr.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hwb.yonumen.top

[R73] 分割大日志
来源：http://lma.mhx1999.top

split -l 1000 big.log part_
来源：http://knp.gotoacloud.top

[R74] 批量重命名
来源：http://cxf.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://per.chenjidiqi.icu

[R75] 导出环境变量
来源：http://ral.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://hdj.yfazqb.com

[R76] 使用临时文件
来源：http://jfk.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jog.yangfankeji.com

[R77] 读取用户输入
来源：http://fmo.nwbrower.top

read -rp "请输入: " ans
来源：http://gga.sweek.top

[R78] 交互式菜单
来源：http://bdy.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://otz.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://seo.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kjz.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://lhg.jyoumei.cn

time ./run.sh
来源：http://ohs.bbcook.cn

================================================================================
来源：http://yqd.chenjidiqi.icu

S. C / C++ 专题
来源：http://uad.hysaishi.cn

================================================================================
来源：http://pla.sysykeji.top

[S01] C：Hello World
来源：http://fbe.jqgfzy.top

#include <stdio.h>
来源：http://mrz.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rfs.tarul.cn

[S02] C：变量与格式化输出
来源：http://aou.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://ysc.havefunace.top

[S03] C：读入整数
来源：http://vgz.xylfe.cn

int x; scanf("%d", &x);
来源：http://yoo.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://aht.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://pws.yj20258.top

[S05] C：字符串长度
来源：http://swu.hammf.cn

strlen(s)
来源：http://eem.pengpengdd.cyou

[S06] C：字符串比较
来源：http://nen.bbcook.cn

strcmp(a, b) == 0
来源：http://dzx.fktsv.cn

[S07] C：数组遍历求和
来源：http://rww.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uys.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://kqx.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pxu.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://hgv.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sej.cheryme.top

[S10] C：指针与解引用
来源：http://xug.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://fmd.guowangkeji.top

[S11] C：逐行读文件
来源：http://onv.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://llq.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://hls.nanxuanxn.top

fclose(f);
来源：http://zen.fanxiaobao.xyz

[S12] C：写文件
来源：http://yxr.pycfn.com


<!-- 参考信息 -->