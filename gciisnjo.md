代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://jhx.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bsd.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://ypg.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xkf.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://cri.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qsc.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://bam.hcnkem.com

[Q49] 更新单行
来源：http://hiw.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://auo.wangdashe.top

[Q50] 批量更新
来源：http://ljo.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qxq.ctjpmb.com

[Q51] 用子查询更新
来源：http://qcb.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zbr.hfpthk.cn

[Q52] 删除指定行
来源：http://cqj.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://bji.birdmap.top

[Q53] 按条件删除
来源：http://gbg.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jph.pycfn.com

[Q54] 清空表
来源：http://jlx.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://idy.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://cal.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zbv.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://ahi.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://koi.nanxuanxn.top

[Q57] 行号
来源：http://qdk.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qyr.gogol.net.cn

[Q58] 累计求和
来源：http://trj.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lmz.pycfn.com

[Q59] 分组内累计
来源：http://yqk.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tqb.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://ojz.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ryq.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rfy.cucudq.cn

[Q61] 移动平均
来源：http://pny.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rnq.ybcxt.top

[Q62] 分组占比
来源：http://bic.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ttp.hfpthk.cn

[Q63] 开启事务
来源：http://rwv.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vmm.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://slo.sufxvd.cn

COMMIT;
来源：http://wnr.ehwqpu.com

[Q65] 回滚事务
来源：http://zyz.bjfxy.top

ROLLBACK;
来源：http://pxd.yueranfly.top

[Q66] 行锁查询
来源：http://qqb.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tqd.daxiang520.top

[Q67] 设置隔离级别
来源：http://anv.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dbw.tanke756.top

[Q68] 保存点
来源：http://nja.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://fvi.ppjwa.cn

ROLLBACK TO sp1;
来源：http://xvc.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://ffn.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yuv.jqgufenzy.top

[Q70] 更新统计信息
来源：http://tma.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://wsy.nanxinkj.top

[Q71] 查看建表语句
来源：http://rry.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fec.yfazqb.com

[Q72] 查看索引
来源：http://biy.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://ezy.jiagoushi.top

[Q73] 查看表状态
来源：http://wkq.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vcc.zycfv.cn

[Q74] 强制使用索引
来源：http://kkt.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zci.birdmap.top

[Q75] 日期格式化
来源：http://uka.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ead.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dum.havefunace.top

[Q76] 按天统计
来源：http://hjv.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gkq.vehdjk.com

[Q77] 时间加减
来源：http://iyq.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jzn.hfpthk.cn

[Q78] 当前时间
来源：http://oxq.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ynx.kuanghao11.cn

[Q79] 字符串拼接
来源：http://uhb.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kbm.xylfe.cn

[Q80] 字符串截取
来源：http://uxs.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blt.sweek.top

[Q81] 字符串替换
来源：http://lww.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://srj.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://koh.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nvn.ivvv.top

[Q83] 大小写转换
来源：http://pqo.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://neh.hesvh.cn

[Q84] 去除首尾空格
来源：http://lee.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://hbw.jianghu66.top

[Q85] 数值取整
来源：http://cgy.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ozu.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://xmm.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ctt.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://ilt.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://exy.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://ozh.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://caz.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uaz.dashuyun.cn

[Q89] 判断表是否存在
来源：http://osx.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rab.zhijiandao.cn

[Q90] 生成序号列
来源：http://ter.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://apg.yj20258.top

================================================================================
来源：http://wew.0kj1m.cn

R. Bash 专题
来源：http://wka.mhx1999.top

================================================================================
来源：http://ozz.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://lel.jinqigufen.top

#!/usr/bin/env bash
来源：http://vty.gogol.net.cn

set -euo pipefail
来源：http://ltl.vehdjk.com

[R02] 变量赋值与使用
来源：http://emw.vehdjk.com

name="Tom"; echo "$name"
来源：http://mmr.zhijiandao.cn

[R03] 只读变量
来源：http://wyi.fengsongda.top

readonly PI=3.14
来源：http://qsa.wangdashe.top

[R04] 位置参数
来源：http://kgh.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xhj.jinqigufen.top

[R05] 参数默认值
来源：http://mfg.jinqigfzy.top

name="${1:-default}"
来源：http://fmq.zhixingplan.top

[R06] 判断命令是否存在
来源：http://dxp.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://erh.cashguo.top

[R07] if 判断文件
来源：http://ubx.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dkk.iojbl.cn

[R08] 数值比较
来源：http://zmf.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hqd.cashguo.top

[R09] 字符串比较
来源：http://noy.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ccz.fehbvm.com

[R10] 正则匹配
来源：http://uux.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://don.ivvv.top

[R11] case 多分支
来源：http://iky.pycfn.com

case "$1" in
来源：http://mcv.shangyingyoupin.top

start) echo "启动" ;;
来源：http://fxd.xuanzx.com

stop)  echo "停止" ;;
来源：http://fjp.mhx1999.top

*)     echo "未知命令" ;;
来源：http://oon.nwbrower.top

esac
来源：http://jue.shzxlz.cn

[R12] for 遍历文件
来源：http://hzl.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://noq.hcnkem.com

[R13] for 计数循环
来源：http://xsf.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://ezr.iojbl.cn

[R14] C 风格 for
来源：http://fpj.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fvt.yj20258.top

[R15] while 逐行读文件
来源：http://qvc.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://glr.cashguo.top

[R16] until 等待条件
来源：http://xuy.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bbp.cdnleiting.top

[R17] 数组定义与取值
来源：http://jmg.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uea.yvedp.cn

[R18] 遍历数组
来源：http://deu.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oqc.vqdsnc.cn

[R19] 数组长度
来源：http://wfe.kuanghao11.cn

echo "${#arr[@]}"
来源：http://qek.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://fik.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xrw.vehdjk.com

[R21] 字符串长度
来源：http://xmc.shanyushiyangkeji.top

echo "${#s}"
来源：http://kih.zhaomingkeji.xyz

[R22] 截取子串
来源：http://ncw.nanxinkj.top

echo "${s:0:5}"
来源：http://ntk.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://gcr.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wgb.chenlongwang.top

[R24] 大小写转换
来源：http://qdz.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://aci.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://hmz.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zsz.aibaodan.cn

[R26] 命令替换
来源：http://cmr.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://ypm.dashuyun.cn

[R27] 算术展开
来源：http://jvp.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://iom.zdbjq.cn

[R28] 浮点运算
来源：http://nmi.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://eip.vqdsnc.cn

[R29] 定义函数
来源：http://wsq.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yty.tianlin.xyz

[R30] 函数返回状态码
来源：http://ijq.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://kcw.jqgfzy.top

[R31] 局部变量
来源：http://fgw.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://jur.chenzaomai.com

[R32] 参数个数校验
来源：http://cbs.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mqq.meibo888.top

[R33] 捕获错误并提示行号
来源：http://dpz.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ibp.jinghuilouyu.cn

[R34] 退出时清理
来源：http://xfj.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://lpr.gotoacloud.top

[R35] 后台执行并等待
来源：http://brd.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lqq.mhx1999.top

[R36] 并发执行多个任务
来源：http://fmf.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mvl.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://aiw.zdqjudy.top

files=$(ls -1)
来源：http://mkn.316326.xyz

[R38] 管道串联
来源：http://fxa.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://uad.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://zwq.jiagoushi.top

cmd > out.log 2>&1
来源：http://hfg.xinyue.icu

[R40] 追加写日志
来源：http://hlp.zhijiandao.cn

echo "log" >> out.log
来源：http://hwx.shzxlz.cn

[R41] 丢弃输出
来源：http://une.aibaodan.cn

cmd >/dev/null 2>&1
来源：http://koh.pycfn.com

[R42] 输入重定向
来源：http://kvl.hammf.cn

wc -l < a.txt
来源：http://fcc.ctjpmb.com

[R43] 按名字查找文件
来源：http://uzj.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://hzy.yanxiufei.cn

[R44] 按修改时间查找
来源：http://pja.yueranfly.top

find . -mtime -7 -type f
来源：http://hlj.316326.xyz

[R45] 批量删除
来源：http://wlk.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://ref.xylfe.cn

[R46] 递归替换文件内容
来源：http://bxk.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxg.jinqigfzy.top

[R47] sed 单行替换
来源：http://cnr.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://xmc.tarul.cn

[R48] awk 取指定列
来源：http://jor.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://yhl.sufxvd.cn

[R49] awk 带条件
来源：http://itr.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cux.fanxiaobao.xyz

[R50] awk 求和
来源：http://imj.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nla.zycfv.cn

[R51] 排序去重取前几
来源：http://owo.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wde.zhoulong.xyz

[R52] 统计行数
来源：http://sca.yueranfly.top

wc -l a.txt
来源：http://ubn.havefunace.top

[R53] 查看文件头与实时尾
来源：http://nlu.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bts.yongpay.top

[R54] 比较两个文件
来源：http://nod.ivvv.top

diff a.txt b.txt
来源：http://kbg.zhoulong.xyz

[R55] 压缩与解压
来源：http://hch.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vie.chenjidiqi.icu

[R56] 远程拷贝
来源：http://lad.gogol.net.cn

scp file user@host:/path/
来源：http://tqu.vehdjk.com

[R57] 远程执行命令
来源：http://psb.aizwys.cn

ssh user@host 'uptime'
来源：http://zdo.xziqi.cn

[R58] 下载文件
来源：http://cbo.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pjf.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://htd.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://apy.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://txk.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fxr.sufxvd.cn

[R61] 磁盘占用
来源：http://egx.zhoulong.xyz

df -h;  du -sh *
来源：http://igj.daria6918.cn

[R62] 找最占空间的文件
来源：http://uad.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://zqh.cashguo.top

[R63] 内存与进程
来源：http://bto.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://kjq.hnqzz.top

[R64] 结束进程
来源：http://ecu.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://vms.pengpengdd.cyou

[R65] 查看端口占用
来源：http://qaz.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oke.yj202588.top

[R66] 定时任务
来源：http://hwc.yongpay.top

crontab -e;  crontab -l
来源：http://cnq.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://nbz.jiagoushi.top

openssl rand -hex 16
来源：http://imw.yj202588.top

[R68] 计算文件校验值
来源：http://nti.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ukn.xuetiantiany.cn

[R69] 生成随机密码
来源：http://oak.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://ure.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://vjk.yuxming.cn

date +%s;  date -d @1700000000
来源：http://coq.svipenyu.cn

[R71] 日期格式化
来源：http://rng.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vbw.cdnleiting.top

[R72] 等待端口就绪
来源：http://jpf.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pyy.tian-w.cn

[R73] 分割大日志
来源：http://grr.hnqzz.top

split -l 1000 big.log part_
来源：http://jzu.ydzc1.top

[R74] 批量重命名
来源：http://vfi.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://esq.yonumen.top

[R75] 导出环境变量
来源：http://ijf.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://tnu.chenzaomai.com

[R76] 使用临时文件
来源：http://dwz.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qat.vqdsnc.cn

[R77] 读取用户输入
来源：http://jsm.hnqzz.top

read -rp "请输入: " ans
来源：http://suy.daxiang520.top

[R78] 交互式菜单
来源：http://wpw.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zjg.aibaodan.cn

[R79] 解析命令行选项
来源：http://vlf.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dvs.birdmap.top

[R80] 查看脚本执行耗时
来源：http://vaf.hnxiangtu.top

time ./run.sh
来源：http://zlo.xinyue.icu

================================================================================
来源：http://mrn.yanxiufei.cn

S. C / C++ 专题
来源：http://lbz.xinyue.icu

================================================================================
来源：http://iet.zhongyouzk.top

[S01] C：Hello World
来源：http://kgi.epnwcf.com

#include <stdio.h>
来源：http://tkf.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wtl.fehbvm.com

[S02] C：变量与格式化输出
来源：http://oxj.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://rwb.yuxming.cn

[S03] C：读入整数
来源：http://run.ybcxt.top

int x; scanf("%d", &x);
来源：http://ipx.jyoumei.cn

[S04] C：字符串复制
来源：http://gjj.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tfm.svipenyu.cn

[S05] C：字符串长度
来源：http://vdi.xuetiantiany.cn

strlen(s)
来源：http://mrc.mhx1999.top

[S06] C：字符串比较
来源：http://wij.yfazqb.com

strcmp(a, b) == 0
来源：http://nwy.vehdjk.com

[S07] C：数组遍历求和
来源：http://pnl.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zlm.yj202588.top

[S08] C：动态内存分配与释放
来源：http://yta.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cgn.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://gnw.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aus.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://klo.yvedp.cn

int *p = &a;  *p = 5;
来源：http://kxx.quarkkingdee.top

[S11] C：逐行读文件
来源：http://ccz.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://wsa.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bbk.chenzaomai.com

fclose(f);
来源：http://nul.jiagoushi.top

[S12] C：写文件
来源：http://eyy.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mim.yfazqb.com

[S13] C：宏定义
来源：http://cwr.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zuf.aibaodan.cn

[S14] C：枚举
来源：http://bos.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://rgr.c1oappe.top

[S15] C：类型转换
来源：http://lqa.hywenlv.cn

(double) a / b
来源：http://qvc.xuetiantiany.cn

[S16] C：位操作置位
来源：http://zee.jqgfzy.top


<!-- 参考信息 -->