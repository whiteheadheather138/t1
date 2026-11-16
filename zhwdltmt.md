代发 wailian999

[Q44] IN 子查询
来源：http://rit.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wyo.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://rjo.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wiw.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://kut.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhz.quarkkingdee.top

[Q47] 与平均值比较
来源：http://uwg.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eob.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://bfk.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://emk.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://abs.yj20258.top

[Q49] 更新单行
来源：http://tog.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xcx.chenjidiqi.icu

[Q50] 批量更新
来源：http://pfi.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gja.cucudq.cn

[Q51] 用子查询更新
来源：http://eva.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bxl.aibaodan.cn

[Q52] 删除指定行
来源：http://gyy.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://sea.hesvh.cn

[Q53] 按条件删除
来源：http://qhf.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xbt.tanke756.top

[Q54] 清空表
来源：http://ehn.uphjek.com

TRUNCATE TABLE logs;
来源：http://ykb.ybcxt.top

[Q55] 排名（并列占位）
来源：http://ykb.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://llc.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://txx.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uxp.ydjk.org.cn

[Q57] 行号
来源：http://rhw.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cby.hfpthk.cn

[Q58] 累计求和
来源：http://igo.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ood.yongpay.top

[Q59] 分组内累计
来源：http://sey.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fio.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://yth.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jyn.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qco.yvedp.cn

[Q61] 移动平均
来源：http://faq.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iuf.jqgfzy.top

[Q62] 分组占比
来源：http://qst.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rdz.mhx1999.top

[Q63] 开启事务
来源：http://sxs.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://orm.guannengcc.top

[Q64] 提交事务
来源：http://kdd.xuanzx.com

COMMIT;
来源：http://spa.bbcook.cn

[Q65] 回滚事务
来源：http://nyz.yfazqb.com

ROLLBACK;
来源：http://vbh.hysaishi.cn

[Q66] 行锁查询
来源：http://vwy.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dlf.zycfv.cn

[Q67] 设置隔离级别
来源：http://cwp.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ruw.cheryme.top

[Q68] 保存点
来源：http://zni.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://zhm.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://ccm.dianchejie.cn

[Q69] 查看执行计划
来源：http://bcs.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cmp.316326.xyz

[Q70] 更新统计信息
来源：http://oju.zhixingplan.top

ANALYZE TABLE users;
来源：http://bbb.chenlongwang.top

[Q71] 查看建表语句
来源：http://dns.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nua.zycfv.cn

[Q72] 查看索引
来源：http://jjh.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://qrf.meibo888.top

[Q73] 查看表状态
来源：http://rco.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wly.dashuyun.cn

[Q74] 强制使用索引
来源：http://iby.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ewh.redwolf501.top

[Q75] 日期格式化
来源：http://gne.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zhx.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vhl.cucudq.cn

[Q76] 按天统计
来源：http://tec.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jlp.zdbjq.cn

[Q77] 时间加减
来源：http://qwa.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kcz.jinqigufen.top

[Q78] 当前时间
来源：http://kid.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ewj.sufxvd.cn

[Q79] 字符串拼接
来源：http://vaf.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://anb.chenjidiqi.icu

[Q80] 字符串截取
来源：http://nup.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nof.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://dum.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://noh.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://owt.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://plj.vehdjk.com

[Q83] 大小写转换
来源：http://oky.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://twd.tian-w.cn

[Q84] 去除首尾空格
来源：http://fcm.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://vgx.gaohongyu789.top

[Q85] 数值取整
来源：http://udz.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvb.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://gov.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sqe.bjfxy.top

[Q87] JSON 字段做条件
来源：http://tdy.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nvy.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://pno.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lmk.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qza.ydzc1.top

[Q89] 判断表是否存在
来源：http://kyj.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ljj.bbcook.cn

[Q90] 生成序号列
来源：http://jsj.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://syk.hfpthk.cn

================================================================================
来源：http://hrf.cqqwz.cn

R. Bash 专题
来源：http://goe.uphjek.com

================================================================================
来源：http://naj.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://bjc.aibaodan.cn

#!/usr/bin/env bash
来源：http://ars.cdnleiting.top

set -euo pipefail
来源：http://ngz.cashguo.top

[R02] 变量赋值与使用
来源：http://tjy.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://cdm.yonumen.top

[R03] 只读变量
来源：http://evg.snrcjt.cn

readonly PI=3.14
来源：http://iiu.yj202588.top

[R04] 位置参数
来源：http://vqn.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wgd.shzxlz.cn

[R05] 参数默认值
来源：http://vzg.cdnleiting.top

name="${1:-default}"
来源：http://jga.ydzc1.top

[R06] 判断命令是否存在
来源：http://kty.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://icc.yonumen.top

[R07] if 判断文件
来源：http://oyl.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hxe.nwbrower.top

[R08] 数值比较
来源：http://set.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ris.xinyue.icu

[R09] 字符串比较
来源：http://nyc.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://upr.gotoacloud.top

[R10] 正则匹配
来源：http://abh.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yqg.zhixingplan.top

[R11] case 多分支
来源：http://gjb.cheryme.top

case "$1" in
来源：http://all.hammf.cn

start) echo "启动" ;;
来源：http://nsn.cdnleiting.top

stop)  echo "停止" ;;
来源：http://osw.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://lyj.xuanzx.com

esac
来源：http://fss.gzhubu.top

[R12] for 遍历文件
来源：http://fnl.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://uyp.hesvh.cn

[R13] for 计数循环
来源：http://yjo.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://gek.wangdashe.top

[R14] C 风格 for
来源：http://jzn.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ets.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://gis.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gjz.shangyingyoupin.top

[R16] until 等待条件
来源：http://dam.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cej.hesvh.cn

[R17] 数组定义与取值
来源：http://rhg.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://uau.yangfankeji.com

[R18] 遍历数组
来源：http://kvv.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xpe.snrcjt.cn

[R19] 数组长度
来源：http://zfo.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://wbq.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://uik.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iac.jianghu66.top

[R21] 字符串长度
来源：http://enz.fktsv.cn

echo "${#s}"
来源：http://nff.vehdjk.com

[R22] 截取子串
来源：http://nst.gogol.net.cn

echo "${s:0:5}"
来源：http://bsr.hcnkem.com

[R23] 字符串替换
来源：http://pet.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sxm.zhongyouzk.top

[R24] 大小写转换
来源：http://yvi.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://zix.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://xlb.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wms.zhengqikj.top

[R26] 命令替换
来源：http://lzn.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://rdc.iojbl.cn

[R27] 算术展开
来源：http://hhw.yongpay.top

echo $((1 + 2 * 3))
来源：http://nff.sxryk.cn

[R28] 浮点运算
来源：http://tme.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://uxs.hcnkem.com

[R29] 定义函数
来源：http://mzl.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mww.chenlongwang.top

[R30] 函数返回状态码
来源：http://lbo.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://fki.tianlin.xyz

[R31] 局部变量
来源：http://bmd.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://vnp.yuxming.cn

[R32] 参数个数校验
来源：http://fah.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpo.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://xaw.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fvj.birdmap.top

[R34] 退出时清理
来源：http://nst.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://eck.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://vxl.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zyy.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://utt.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bjp.sysykeji.top

[R37] 把输出赋给变量
来源：http://njl.fengsongda.top

files=$(ls -1)
来源：http://khk.hnxiangtu.top

[R38] 管道串联
来源：http://qsb.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://qqy.yj202588.top

[R39] 重定向标准输出与错误
来源：http://qnh.ppjwa.cn

cmd > out.log 2>&1
来源：http://hqh.daria6918.cn

[R40] 追加写日志
来源：http://afr.zdbjq.cn

echo "log" >> out.log
来源：http://apc.yangfankeji.com

[R41] 丢弃输出
来源：http://gre.guannengcc.top

cmd >/dev/null 2>&1
来源：http://zwx.jinghuilouyu.cn

[R42] 输入重定向
来源：http://gji.xziqi.cn

wc -l < a.txt
来源：http://tma.yj202588.top

[R43] 按名字查找文件
来源：http://utj.sufxvd.cn

find . -name "*.log" -type f
来源：http://xrf.ctjpmb.com

[R44] 按修改时间查找
来源：http://ubn.zhixingplan.top

find . -mtime -7 -type f
来源：http://ume.nwbrower.top

[R45] 批量删除
来源：http://imc.shuidangran.top

find . -name "*.tmp" -delete
来源：http://rrz.hywenlv.cn

[R46] 递归替换文件内容
来源：http://ntt.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jyi.52xcode.cn

[R47] sed 单行替换
来源：http://kpf.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qzn.ehwqpu.com

[R48] awk 取指定列
来源：http://mug.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://rbp.shanyushiyangtech.top

[R49] awk 带条件
来源：http://doj.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lyw.fktsv.cn

[R50] awk 求和
来源：http://hbw.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://ssf.ydjk.org.cn

[R51] 排序去重取前几
来源：http://kgy.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lis.zdbjq.cn

[R52] 统计行数
来源：http://xbz.ydjk.org.cn

wc -l a.txt
来源：http://tlz.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://fwt.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://snw.jyoumei.cn

[R54] 比较两个文件
来源：http://mkn.yj20258.top

diff a.txt b.txt
来源：http://qqv.zhengqikj.top

[R55] 压缩与解压
来源：http://sgy.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yeu.yuanzhike.top

[R56] 远程拷贝
来源：http://rhu.ydjk.org.cn

scp file user@host:/path/
来源：http://bpz.pengpengdd.cyou

[R57] 远程执行命令
来源：http://txx.c1oappe.top

ssh user@host 'uptime'
来源：http://hag.gaohongyu789.top

[R58] 下载文件
来源：http://vfv.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vnq.xinyue.icu

[R59] 发 POST JSON
来源：http://tld.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zgc.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://nqg.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pza.smart0.xyz

[R61] 磁盘占用
来源：http://hwq.nwbrower.top

df -h;  du -sh *
来源：http://bod.cashguo.top

[R62] 找最占空间的文件
来源：http://lew.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://hdu.xinyue.icu

[R63] 内存与进程
来源：http://uwn.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://qzh.iojbl.cn

[R64] 结束进程
来源：http://osk.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://qoj.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://mhv.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tkr.jiagoushi.top

[R66] 定时任务
来源：http://vnc.jlsjyb.cn

crontab -e;  crontab -l
来源：http://lpf.mhx1999.top

[R67] 生成随机十六进制串
来源：http://cnc.uphjek.com

openssl rand -hex 16
来源：http://hcj.ydzc1.top

[R68] 计算文件校验值
来源：http://xtp.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://xoe.andypj.xyz

[R69] 生成随机密码
来源：http://bbb.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://vgx.guannengcc.top

[R70] 时间戳与互转
来源：http://uva.redwolf501.top

date +%s;  date -d @1700000000
来源：http://ptw.ivvv.top

[R71] 日期格式化
来源：http://vdj.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://npn.gaohongyu789.top

[R72] 等待端口就绪
来源：http://qxl.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://xrg.52xcode.cn

[R73] 分割大日志
来源：http://vii.redwolf501.top

split -l 1000 big.log part_
来源：http://vwq.sxryk.cn

[R74] 批量重命名
来源：http://iij.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zap.smart0.xyz

[R75] 导出环境变量
来源：http://ztn.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://wes.chenzaomai.com

[R76] 使用临时文件
来源：http://vzi.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aeo.vqdsnc.cn

[R77] 读取用户输入
来源：http://xkw.c1oappe.top

read -rp "请输入: " ans
来源：http://umk.yfazqb.com

[R78] 交互式菜单
来源：http://sis.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lrn.ehwqpu.com

[R79] 解析命令行选项
来源：http://aff.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bsj.yj202588.top

[R80] 查看脚本执行耗时
来源：http://rsa.sweek.top

time ./run.sh
来源：http://ejz.feifeiyinyue.top

================================================================================
来源：http://hnx.jinghuilouyu.cn

S. C / C++ 专题
来源：http://gau.ybcxt.top

================================================================================
来源：http://fin.vqdsnc.cn

[S01] C：Hello World
来源：http://ldo.iojbl.cn

#include <stdio.h>
来源：http://ddk.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ggf.fktsv.cn

[S02] C：变量与格式化输出
来源：http://nyp.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://hug.andypj.xyz

[S03] C：读入整数
来源：http://nle.ivvv.top

int x; scanf("%d", &x);
来源：http://bvx.hywenlv.cn

[S04] C：字符串复制
来源：http://mbq.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://new.zhengqikj.top

[S05] C：字符串长度
来源：http://ury.yvedp.cn

strlen(s)
来源：http://zfa.yonumen.top

[S06] C：字符串比较
来源：http://nwp.zhengqikj.top

strcmp(a, b) == 0
来源：http://ppk.bjfxy.top

[S07] C：数组遍历求和
来源：http://jic.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ije.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://uni.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://scc.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://bmh.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qvb.yonumen.top

[S10] C：指针与解引用
来源：http://gmg.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://rda.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://mlc.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://eyw.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://enw.yj202588.top

fclose(f);
来源：http://cjr.cashguo.top

[S12] C：写文件
来源：http://vpo.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cky.kuanghao11.cn

[S13] C：宏定义
来源：http://led.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ryw.jyoumei.cn

[S14] C：枚举
来源：http://rpe.zhixingplan.top


<!-- 参考信息 -->