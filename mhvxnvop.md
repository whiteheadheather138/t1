代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://lxm.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gtd.shzxlz.cn

[Q43] 标量子查询
来源：http://bgl.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hch.hongshengwenyu.top

[Q44] IN 子查询
来源：http://fyo.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kwx.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://mcj.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qtk.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://omo.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://egy.zdqjudy.top

[Q47] 与平均值比较
来源：http://xfm.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mim.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://mcn.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kix.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://azx.tianlin.xyz

[Q49] 更新单行
来源：http://kac.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pgb.cashguo.top

[Q50] 批量更新
来源：http://vpz.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oon.havefunace.top

[Q51] 用子查询更新
来源：http://fvx.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vkb.feifeiyinyue.top

[Q52] 删除指定行
来源：http://dod.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://fwz.jyoumei.cn

[Q53] 按条件删除
来源：http://quz.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qyg.zycfv.cn

[Q54] 清空表
来源：http://dzl.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://qse.andypj.xyz

[Q55] 排名（并列占位）
来源：http://cxq.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ngn.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://bph.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kgz.daxiang520.top

[Q57] 行号
来源：http://chn.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tli.nwbrower.top

[Q58] 累计求和
来源：http://zwu.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kpv.yueranfly.top

[Q59] 分组内累计
来源：http://pxr.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kkb.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://fkz.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dnn.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hwa.meibo888.top

[Q61] 移动平均
来源：http://afu.jianghu66.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wfl.fehbvm.com

[Q62] 分组占比
来源：http://jqs.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://htj.quarkkingdee.top

[Q63] 开启事务
来源：http://yjd.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tjt.aibaodan.cn

[Q64] 提交事务
来源：http://xex.vehdjk.com

COMMIT;
来源：http://ank.ybcxt.top

[Q65] 回滚事务
来源：http://adq.daria6918.cn

ROLLBACK;
来源：http://pxb.jiagoushi.top

[Q66] 行锁查询
来源：http://wsg.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwi.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://vge.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nja.epnwcf.com

[Q68] 保存点
来源：http://aii.sweek.top

SAVEPOINT sp1;
来源：http://cmw.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://mih.jiagoushi.top

[Q69] 查看执行计划
来源：http://xal.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fzb.xziqi.cn

[Q70] 更新统计信息
来源：http://tuj.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://qtn.fzhhl.top

[Q71] 查看建表语句
来源：http://ele.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ajw.ydzc1.top

[Q72] 查看索引
来源：http://zak.sweek.top

SHOW INDEX FROM users;
来源：http://uok.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://gcq.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eih.aibaodan.cn

[Q74] 强制使用索引
来源：http://rld.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cjj.jqgufenzy.top

[Q75] 日期格式化
来源：http://omy.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jwj.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vcu.shuidangran.top

[Q76] 按天统计
来源：http://xlu.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hgo.fktsv.cn

[Q77] 时间加减
来源：http://fky.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zqo.zhixingplan.top

[Q78] 当前时间
来源：http://rfd.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jiw.ybcxt.top

[Q79] 字符串拼接
来源：http://azy.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wct.hammf.cn

[Q80] 字符串截取
来源：http://fyv.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://apq.zycfv.cn

[Q81] 字符串替换
来源：http://mci.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cjg.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://fvv.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qhe.yj20258888.top

[Q83] 大小写转换
来源：http://lvl.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://paq.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://yhj.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://ajp.gzhubu.top

[Q85] 数值取整
来源：http://iil.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yeu.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://ovi.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rwj.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://kqv.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hpv.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://adf.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wax.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wlb.aibaodan.cn

[Q89] 判断表是否存在
来源：http://nhx.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uzj.yangfankeji.com

[Q90] 生成序号列
来源：http://haw.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wvk.ybcxt.top

================================================================================
来源：http://kzo.hesvh.cn

R. Bash 专题
来源：http://ejk.vqdsnc.cn

================================================================================
来源：http://jux.hfpthk.cn

[R01] shebang 与严格模式
来源：http://smg.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://tah.yangfankeji.com

set -euo pipefail
来源：http://lcn.redwolf501.top

[R02] 变量赋值与使用
来源：http://qcj.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://hvx.yanxiufei.cn

[R03] 只读变量
来源：http://mhc.yj202588.top

readonly PI=3.14
来源：http://ayp.meibo888.top

[R04] 位置参数
来源：http://qog.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uoo.epnwcf.com

[R05] 参数默认值
来源：http://pun.shanyushiyangtech.top

name="${1:-default}"
来源：http://fbr.daria6918.cn

[R06] 判断命令是否存在
来源：http://rah.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cnq.sjlbkw.cn

[R07] if 判断文件
来源：http://rfu.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ofj.vqdsnc.cn

[R08] 数值比较
来源：http://twh.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dxo.uphjek.com

[R09] 字符串比较
来源：http://bqn.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://svi.dashuyun.cn

[R10] 正则匹配
来源：http://nes.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kcz.dashuyun.cn

[R11] case 多分支
来源：http://lyk.quarkkingdee.top

case "$1" in
来源：http://mah.hnxiangtu.top

start) echo "启动" ;;
来源：http://qgq.zycfv.cn

stop)  echo "停止" ;;
来源：http://jho.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://cas.wangdashe.top

esac
来源：http://azm.quarkkingdee.top

[R12] for 遍历文件
来源：http://icd.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://etx.xinyue.icu

[R13] for 计数循环
来源：http://njh.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://akq.zdqjudy.top

[R14] C 风格 for
来源：http://ntw.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uxz.yvedp.cn

[R15] while 逐行读文件
来源：http://dqs.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fmk.birdmap.top

[R16] until 等待条件
来源：http://off.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdl.yvedp.cn

[R17] 数组定义与取值
来源：http://xps.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://get.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://hlh.cheryme.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zdi.dianchejie.cn

[R19] 数组长度
来源：http://acr.tianlin.xyz

echo "${#arr[@]}"
来源：http://jrv.birdmap.top

[R20] 关联数组（字典）
来源：http://zhp.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ifm.birdmap.top

[R21] 字符串长度
来源：http://lfd.pycfn.com

echo "${#s}"
来源：http://gko.yvedp.cn

[R22] 截取子串
来源：http://hdi.52xcode.cn

echo "${s:0:5}"
来源：http://jch.shanyushiyangtech.top

[R23] 字符串替换
来源：http://dcv.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jai.yongpay.top

[R24] 大小写转换
来源：http://dui.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://uod.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://zpv.hongshengwenyu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mxx.ctjpmb.com

[R26] 命令替换
来源：http://huj.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://how.jinqigufen.top

[R27] 算术展开
来源：http://rhd.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://gea.316326.xyz

[R28] 浮点运算
来源：http://lpn.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://cgo.zhengqikj.top

[R29] 定义函数
来源：http://ovl.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpk.mhx1999.top

[R30] 函数返回状态码
来源：http://aff.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://spr.fktsv.cn

[R31] 局部变量
来源：http://jpn.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://bmv.zhengqikj.top

[R32] 参数个数校验
来源：http://zgn.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kik.uphjek.com

[R33] 捕获错误并提示行号
来源：http://afl.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hmo.jinghuilouyu.cn

[R34] 退出时清理
来源：http://dwz.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://exd.nanxuanxn.top

[R35] 后台执行并等待
来源：http://egj.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://khe.hfpthk.cn

[R36] 并发执行多个任务
来源：http://ypo.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nos.redwolf501.top

[R37] 把输出赋给变量
来源：http://vrd.cucudq.cn

files=$(ls -1)
来源：http://ptq.jinyuanbaomall.cn

[R38] 管道串联
来源：http://qwa.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://psc.ivvv.top

[R39] 重定向标准输出与错误
来源：http://rzi.kuanghao11.cn

cmd > out.log 2>&1
来源：http://lqq.shanyushiyangtech.top

[R40] 追加写日志
来源：http://uro.zdbjq.cn

echo "log" >> out.log
来源：http://ytj.ppjwa.cn

[R41] 丢弃输出
来源：http://tqs.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://uhu.tianlin.xyz

[R42] 输入重定向
来源：http://wlf.bjfxy.top

wc -l < a.txt
来源：http://vyk.c1oappe.top

[R43] 按名字查找文件
来源：http://knz.yuanzhike.top

find . -name "*.log" -type f
来源：http://wew.hywenlv.cn

[R44] 按修改时间查找
来源：http://shz.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://dsb.ppjwa.cn

[R45] 批量删除
来源：http://ibd.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://gsg.9152youxi.cn

[R46] 递归替换文件内容
来源：http://snl.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hyj.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://ogi.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://lnn.fehbvm.com

[R48] awk 取指定列
来源：http://yph.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://nnz.havefunace.top

[R49] awk 带条件
来源：http://pnw.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gmy.hywenlv.cn

[R50] awk 求和
来源：http://iqp.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bsa.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://zzo.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ksp.quarkkingdee.top

[R52] 统计行数
来源：http://wpp.fanxiaobao.xyz

wc -l a.txt
来源：http://mih.jianghu66.top

[R53] 查看文件头与实时尾
来源：http://vjr.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hcl.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://oau.jqgufenzy.top

diff a.txt b.txt
来源：http://ijy.bjfxy.top

[R55] 压缩与解压
来源：http://cgw.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iva.fengsongda.top

[R56] 远程拷贝
来源：http://vxy.haohaochexian.top

scp file user@host:/path/
来源：http://lsd.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://tvf.shzxlz.cn

ssh user@host 'uptime'
来源：http://fhu.zycfv.cn

[R58] 下载文件
来源：http://zzv.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jaw.vqdsnc.cn

[R59] 发 POST JSON
来源：http://imp.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qdj.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://eyb.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tgt.ybcxt.top

[R61] 磁盘占用
来源：http://kfy.pycfn.com

df -h;  du -sh *
来源：http://lns.0kj1m.cn

[R62] 找最占空间的文件
来源：http://qja.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://rxl.xuanzx.com

[R63] 内存与进程
来源：http://bdj.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://par.cqqwz.cn

[R64] 结束进程
来源：http://rvd.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://szl.tarul.cn

[R65] 查看端口占用
来源：http://vnp.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovy.yvedp.cn

[R66] 定时任务
来源：http://krr.havefunace.top

crontab -e;  crontab -l
来源：http://nsa.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://rwn.sufxvd.cn

openssl rand -hex 16
来源：http://azk.hnxiangtu.top

[R68] 计算文件校验值
来源：http://run.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ryn.jqgfzy.top

[R69] 生成随机密码
来源：http://oer.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://ntt.nwbrower.top

[R70] 时间戳与互转
来源：http://dfy.yongpay.top

date +%s;  date -d @1700000000
来源：http://zlk.birdmap.top

[R71] 日期格式化
来源：http://qpp.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lca.jinqigfzy.top

[R72] 等待端口就绪
来源：http://zsy.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dzt.gaohongyu789.top

[R73] 分割大日志
来源：http://vud.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://hju.52xcode.cn

[R74] 批量重命名
来源：http://ame.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zpk.shuidangran.top

[R75] 导出环境变量
来源：http://gur.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://xkr.zycfv.cn

[R76] 使用临时文件
来源：http://osw.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nlz.vqdsnc.cn

[R77] 读取用户输入
来源：http://lmi.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://bkg.nanxuanxn.top

[R78] 交互式菜单
来源：http://uyr.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://wpe.bjfxy.top

[R79] 解析命令行选项
来源：http://xkk.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nwe.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://mqq.havefunace.top

time ./run.sh
来源：http://uqh.yj20258.top

================================================================================
来源：http://mjz.yj20258.top

S. C / C++ 专题
来源：http://deg.jqgufenzy.top

================================================================================
来源：http://gmr.0kj1m.cn

[S01] C：Hello World
来源：http://gxx.gaohongyu789.top

#include <stdio.h>
来源：http://wiy.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zju.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://kgm.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://wub.cheryme.top

[S03] C：读入整数
来源：http://ilo.ppjwa.cn

int x; scanf("%d", &x);
来源：http://jys.daxiang520.top

[S04] C：字符串复制
来源：http://jdq.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://cxp.xziqi.cn

[S05] C：字符串长度
来源：http://iqq.zdbjq.cn

strlen(s)
来源：http://ggz.hnqzz.top

[S06] C：字符串比较
来源：http://cbp.gaohongyu789.top

strcmp(a, b) == 0
来源：http://vix.sxryk.cn

[S07] C：数组遍历求和
来源：http://jnn.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ycm.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://kty.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eds.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://kqg.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://itg.ydjk.org.cn

[S10] C：指针与解引用
来源：http://sfj.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://ksa.daria6918.cn

[S11] C：逐行读文件
来源：http://lrh.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://fni.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jhk.jqgfzy.top

fclose(f);
来源：http://kzj.cashguo.top

[S12] C：写文件
来源：http://tjg.cashguo.top


<!-- 参考信息 -->