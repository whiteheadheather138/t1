代发 wailian999

[Q44] IN 子查询
来源：http://whf.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lxp.snrcjt.cn

[Q45] EXISTS 判断存在
来源：http://krn.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xrz.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nfn.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hiu.zhengqikj.top

[Q47] 与平均值比较
来源：http://sfb.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xcv.tarul.cn

[Q48] CTE 公用表表达式
来源：http://tng.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://swn.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://yfn.tarul.cn

[Q49] 更新单行
来源：http://lnw.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aoo.sxryk.cn

[Q50] 批量更新
来源：http://mpv.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wub.smart0.xyz

[Q51] 用子查询更新
来源：http://ufm.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://psu.ctjpmb.com

[Q52] 删除指定行
来源：http://mmt.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://glc.ybcxt.top

[Q53] 按条件删除
来源：http://zcg.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tun.yvedp.cn

[Q54] 清空表
来源：http://kid.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://jdp.yj202588.top

[Q55] 排名（并列占位）
来源：http://afq.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ucq.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://eft.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vbf.jqgfzy.top

[Q57] 行号
来源：http://goa.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ehl.ydzc1.top

[Q58] 累计求和
来源：http://wuk.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ubq.zycfv.cn

[Q59] 分组内累计
来源：http://oyp.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zuo.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://dnn.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ykr.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fuk.aibaodan.cn

[Q61] 移动平均
来源：http://yjj.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bia.yfazqb.com

[Q62] 分组占比
来源：http://lfc.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://siu.yj202588.top

[Q63] 开启事务
来源：http://ubq.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ikj.chenjidiqi.icu

[Q64] 提交事务
来源：http://lcz.vehdjk.com

COMMIT;
来源：http://nou.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://acl.shangyingyoupin.top

ROLLBACK;
来源：http://gol.ybcxt.top

[Q66] 行锁查询
来源：http://jwh.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pso.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://wmy.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xkc.havefunace.top

[Q68] 保存点
来源：http://gff.meibo888.top

SAVEPOINT sp1;
来源：http://oiq.chenzaomai.com

ROLLBACK TO sp1;
来源：http://dyh.kuanghao11.cn

[Q69] 查看执行计划
来源：http://yfn.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mtu.ydjk.org.cn

[Q70] 更新统计信息
来源：http://wjo.jlsjyb.cn

ANALYZE TABLE users;
来源：http://iuz.nanxinkj.top

[Q71] 查看建表语句
来源：http://ggl.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zwr.iojbl.cn

[Q72] 查看索引
来源：http://pkl.mhx1999.top

SHOW INDEX FROM users;
来源：http://gxz.daxiang520.top

[Q73] 查看表状态
来源：http://qoo.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uye.epnwcf.com

[Q74] 强制使用索引
来源：http://ugh.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sdt.yangfankeji.com

[Q75] 日期格式化
来源：http://rne.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qnp.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iuk.epnwcf.com

[Q76] 按天统计
来源：http://rex.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fne.sjlbkw.cn

[Q77] 时间加减
来源：http://yan.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lyk.yanxiufei.cn

[Q78] 当前时间
来源：http://bmp.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nay.fengsongda.top

[Q79] 字符串拼接
来源：http://hfl.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tnw.jinqigufen.top

[Q80] 字符串截取
来源：http://nbm.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ieq.fengsongda.top

[Q81] 字符串替换
来源：http://rdj.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kte.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://xtb.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://abx.daria6918.cn

[Q83] 大小写转换
来源：http://lzo.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lym.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://rxl.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://ncr.xziqi.cn

[Q85] 数值取整
来源：http://gxj.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wzh.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://rsu.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lmz.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://pnq.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xix.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://imq.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yxu.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ciq.sxryk.cn

[Q89] 判断表是否存在
来源：http://jho.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zvc.daria6918.cn

[Q90] 生成序号列
来源：http://mhg.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wtf.yongpay.top

================================================================================
来源：http://lrl.iojbl.cn

R. Bash 专题
来源：http://pcr.shanyushiyangkeji.top

================================================================================
来源：http://rzg.hfpthk.cn

[R01] shebang 与严格模式
来源：http://mlg.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://iun.cdnleiting.top

set -euo pipefail
来源：http://jtq.snrcjt.cn

[R02] 变量赋值与使用
来源：http://wck.hesvh.cn

name="Tom"; echo "$name"
来源：http://gma.chenjidiqi.icu

[R03] 只读变量
来源：http://vwd.pengpengdd.cyou

readonly PI=3.14
来源：http://sqc.yvedp.cn

[R04] 位置参数
来源：http://rcu.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wgi.feifeiyinyue.top

[R05] 参数默认值
来源：http://zlj.fanxiaobao.xyz

name="${1:-default}"
来源：http://enm.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://hng.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wyz.haohaochexian.top

[R07] if 判断文件
来源：http://wpq.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xuh.jinqigfzy.top

[R08] 数值比较
来源：http://mpo.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vki.smart0.xyz

[R09] 字符串比较
来源：http://zfj.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jom.smart0.xyz

[R10] 正则匹配
来源：http://lpw.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://odl.meibo888.top

[R11] case 多分支
来源：http://uid.pengpengdd.cyou

case "$1" in
来源：http://qgw.yj20258888.top

start) echo "启动" ;;
来源：http://xog.yuanzhike.top

stop)  echo "停止" ;;
来源：http://izp.aizwys.cn

*)     echo "未知命令" ;;
来源：http://lkv.ydjk.org.cn

esac
来源：http://zob.pengpengdd.cyou

[R12] for 遍历文件
来源：http://rcy.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://mym.andypj.xyz

[R13] for 计数循环
来源：http://spv.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://sec.yanxiufei.cn

[R14] C 风格 for
来源：http://afs.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pab.sweek.top

[R15] while 逐行读文件
来源：http://yju.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vdc.tarul.cn

[R16] until 等待条件
来源：http://eew.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://txo.cheryme.top

[R17] 数组定义与取值
来源：http://aae.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://kgk.9152youxi.cn

[R18] 遍历数组
来源：http://dik.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vfm.ydjk.org.cn

[R19] 数组长度
来源：http://wxw.xylfe.cn

echo "${#arr[@]}"
来源：http://yfl.9152youxi.cn

[R20] 关联数组（字典）
来源：http://ebe.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ply.zhongyouzk.top

[R21] 字符串长度
来源：http://evg.havefunace.top

echo "${#s}"
来源：http://pry.xingfuxueyuan.xyz

[R22] 截取子串
来源：http://xtn.aibaodan.cn

echo "${s:0:5}"
来源：http://mle.zhijiandao.cn

[R23] 字符串替换
来源：http://ire.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://trg.uphjek.com

[R24] 大小写转换
来源：http://uyw.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://woa.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://fxb.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fpx.pycfn.com

[R26] 命令替换
来源：http://ssc.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://kky.yanxiufei.cn

[R27] 算术展开
来源：http://lrj.c1oappe.top

echo $((1 + 2 * 3))
来源：http://meb.yvedp.cn

[R28] 浮点运算
来源：http://gwk.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://dhk.ydjk.org.cn

[R29] 定义函数
来源：http://zbj.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://grc.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://mkp.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://pfc.shangyingyoupin.top

[R31] 局部变量
来源：http://ltw.sweek.top

f() { local x=1; echo "$x"; }
来源：http://qfh.smart0.xyz

[R32] 参数个数校验
来源：http://nek.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xgf.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://nmb.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gdc.yj20258888.top

[R34] 退出时清理
来源：http://qzh.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://kzp.zhijiandao.cn

[R35] 后台执行并等待
来源：http://dmf.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rpa.yuxming.cn

[R36] 并发执行多个任务
来源：http://aol.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wre.daxiang520.top

[R37] 把输出赋给变量
来源：http://gqj.sweek.top

files=$(ls -1)
来源：http://osy.ctjpmb.com

[R38] 管道串联
来源：http://zpb.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://flj.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://thh.tian-w.cn

cmd > out.log 2>&1
来源：http://ahf.hnxiangtu.top

[R40] 追加写日志
来源：http://pgw.yueranfly.top

echo "log" >> out.log
来源：http://dhr.jqgfzy.top

[R41] 丢弃输出
来源：http://nhd.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://vqs.dashuyun.cn

[R42] 输入重定向
来源：http://bas.andypj.xyz

wc -l < a.txt
来源：http://amd.pycfn.com

[R43] 按名字查找文件
来源：http://qqk.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://mtr.gogol.net.cn

[R44] 按修改时间查找
来源：http://ydt.zhijiandao.cn

find . -mtime -7 -type f
来源：http://dee.fzhhl.top

[R45] 批量删除
来源：http://kbb.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://icp.nwbrower.top

[R46] 递归替换文件内容
来源：http://lne.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kfn.iojbl.cn

[R47] sed 单行替换
来源：http://fxf.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://zir.zhixingplan.top

[R48] awk 取指定列
来源：http://bnn.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://wxo.zhoulong.xyz

[R49] awk 带条件
来源：http://zzz.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oau.guannengcc.top

[R50] awk 求和
来源：http://ljn.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://rqu.316326.xyz

[R51] 排序去重取前几
来源：http://mnc.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eue.sysykeji.top

[R52] 统计行数
来源：http://rlh.jianghu66.top

wc -l a.txt
来源：http://ohr.uphjek.com

[R53] 查看文件头与实时尾
来源：http://jvz.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jrk.ppjwa.cn

[R54] 比较两个文件
来源：http://gbv.daria6918.cn

diff a.txt b.txt
来源：http://sto.hesvh.cn

[R55] 压缩与解压
来源：http://ovq.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ftu.jyoumei.cn

[R56] 远程拷贝
来源：http://rww.tanke756.top

scp file user@host:/path/
来源：http://qbd.c1oappe.top

[R57] 远程执行命令
来源：http://mwp.0kj1m.cn

ssh user@host 'uptime'
来源：http://elm.zhaomingkeji.xyz

[R58] 下载文件
来源：http://cuw.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aow.yueranfly.top

[R59] 发 POST JSON
来源：http://uez.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tvm.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://jon.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://clu.xuanzx.com

[R61] 磁盘占用
来源：http://kuo.0kj1m.cn

df -h;  du -sh *
来源：http://bty.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://sfx.pycfn.com

du -ah . | sort -rh | head -10
来源：http://tku.daria6918.cn

[R63] 内存与进程
来源：http://qzk.yj202588.top

free -h;  ps aux | grep nginx
来源：http://cgz.dashuyun.cn

[R64] 结束进程
来源：http://czu.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://dgq.dianchejie.cn

[R65] 查看端口占用
来源：http://wov.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gzf.zhiwuduotai.top

[R66] 定时任务
来源：http://qyh.tian-w.cn

crontab -e;  crontab -l
来源：http://yrz.yj20258888.top

[R67] 生成随机十六进制串
来源：http://fyr.wangshuangyany.cn

openssl rand -hex 16
来源：http://dgw.nanxinkj.top

[R68] 计算文件校验值
来源：http://tuc.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://zdy.wangdashe.top

[R69] 生成随机密码
来源：http://sze.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://jmk.bjfxy.top

[R70] 时间戳与互转
来源：http://oev.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://hwl.jqgfzy.top

[R71] 日期格式化
来源：http://rbc.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bvx.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://zsj.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://slh.nwbrower.top

[R73] 分割大日志
来源：http://oxm.dashuyun.cn

split -l 1000 big.log part_
来源：http://hdc.hesvh.cn

[R74] 批量重命名
来源：http://keu.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pfo.nwbrower.top

[R75] 导出环境变量
来源：http://jez.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://agf.meibo888.top

[R76] 使用临时文件
来源：http://fmg.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tny.aizwys.cn

[R77] 读取用户输入
来源：http://sxv.ydzc1.top

read -rp "请输入: " ans
来源：http://tlg.tianlin.xyz

[R78] 交互式菜单
来源：http://klz.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ojl.iojbl.cn

[R79] 解析命令行选项
来源：http://mgq.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ecc.tarul.cn

[R80] 查看脚本执行耗时
来源：http://nbw.tarul.cn

time ./run.sh
来源：http://yzp.jyoumei.cn

================================================================================
来源：http://wxg.dianchejie.cn

S. C / C++ 专题
来源：http://pfk.yj20258888.top

================================================================================
来源：http://iat.havefunace.top

[S01] C：Hello World
来源：http://pjj.ywan-chungtsiang.top

#include <stdio.h>
来源：http://hbf.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xev.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://mij.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://box.hnqzz.top

[S03] C：读入整数
来源：http://tel.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://fyo.0kj1m.cn

[S04] C：字符串复制
来源：http://osm.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wdu.guannengcc.top

[S05] C：字符串长度
来源：http://mub.zycfv.cn

strlen(s)
来源：http://fcv.hammf.cn

[S06] C：字符串比较
来源：http://bjl.yj20258.top

strcmp(a, b) == 0
来源：http://ofh.vehdjk.com

[S07] C：数组遍历求和
来源：http://sgd.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eyq.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://vow.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ats.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://czq.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rjn.gaohongyu789.top

[S10] C：指针与解引用
来源：http://xdy.pycfn.com

int *p = &a;  *p = 5;
来源：http://lul.daria6918.cn

[S11] C：逐行读文件
来源：http://cjj.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://yxc.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgy.jianghu66.top

fclose(f);
来源：http://blt.fengsongda.top

[S12] C：写文件
来源：http://nyy.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixf.zhengqikj.top

[S13] C：宏定义
来源：http://elu.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xyx.fanxiaobao.xyz

[S14] C：枚举
来源：http://jxv.zycfv.cn


<!-- 参考信息 -->