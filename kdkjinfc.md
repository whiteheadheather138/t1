代发 wailian999

[Q44] IN 子查询
来源：http://lzd.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xfc.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://pzx.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mii.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://znc.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://moz.epnwcf.com

[Q47] 与平均值比较
来源：http://hwt.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nvl.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://quj.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jrn.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://mod.nwbrower.top

[Q49] 更新单行
来源：http://uwt.cucudq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qaw.andypj.xyz

[Q50] 批量更新
来源：http://mhj.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rxs.jiagoushi.top

[Q51] 用子查询更新
来源：http://fnu.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://egh.tianlin.xyz

[Q52] 删除指定行
来源：http://beq.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://apv.xylfe.cn

[Q53] 按条件删除
来源：http://dmj.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gku.hfpthk.cn

[Q54] 清空表
来源：http://myl.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://dcy.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://aml.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://luq.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://fem.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qtg.hammf.cn

[Q57] 行号
来源：http://yga.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lmu.yj20258888.top

[Q58] 累计求和
来源：http://rtj.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wjl.zhixingplan.top

[Q59] 分组内累计
来源：http://vbj.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pgh.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://xkn.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ncc.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ntc.tian-w.cn

[Q61] 移动平均
来源：http://yjf.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qin.ivvv.top

[Q62] 分组占比
来源：http://ife.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bec.jianghu66.top

[Q63] 开启事务
来源：http://div.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://hzs.aizwys.cn

[Q64] 提交事务
来源：http://nnm.xingfuxueyuan.xyz

COMMIT;
来源：http://xpe.jlsjyb.cn

[Q65] 回滚事务
来源：http://gfs.sufxvd.cn

ROLLBACK;
来源：http://cgv.jiagoushi.top

[Q66] 行锁查询
来源：http://gpe.hysaishi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mev.iojbl.cn

[Q67] 设置隔离级别
来源：http://hud.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yrz.jinqigufen.top

[Q68] 保存点
来源：http://lkq.sjlbkw.cn

SAVEPOINT sp1;
来源：http://yjr.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://yyv.nanxuanxn.top

[Q69] 查看执行计划
来源：http://ups.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uty.zhongyouzk.top

[Q70] 更新统计信息
来源：http://tjt.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://kwy.svipenyu.cn

[Q71] 查看建表语句
来源：http://czl.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://piw.vqdsnc.cn

[Q72] 查看索引
来源：http://ofn.gzhubu.top

SHOW INDEX FROM users;
来源：http://huk.epnwcf.com

[Q73] 查看表状态
来源：http://bks.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dhr.yj20258888.top

[Q74] 强制使用索引
来源：http://lch.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jom.zhongyouzk.top

[Q75] 日期格式化
来源：http://hho.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gro.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qwb.zhoulong.xyz

[Q76] 按天统计
来源：http://nwo.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ais.wangshuangyany.cn

[Q77] 时间加减
来源：http://aqo.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tem.chenjidiqi.icu

[Q78] 当前时间
来源：http://wef.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ato.yonumen.top

[Q79] 字符串拼接
来源：http://sid.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hsl.meibo888.top

[Q80] 字符串截取
来源：http://scf.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ptw.bjfxy.top

[Q81] 字符串替换
来源：http://mfd.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lul.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://box.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fpb.zdqjudy.top

[Q83] 大小写转换
来源：http://ifc.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pdi.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://agh.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://szs.cucudq.cn

[Q85] 数值取整
来源：http://uvb.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tgy.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://fqg.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jxz.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://jvw.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jia.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://bec.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpi.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kdp.cheryme.top

[Q89] 判断表是否存在
来源：http://qdc.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rbb.yvedp.cn

[Q90] 生成序号列
来源：http://ynr.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yuh.xziqi.cn

================================================================================
来源：http://lkz.ybcxt.top

R. Bash 专题
来源：http://jyf.9152youxi.cn

================================================================================
来源：http://pnp.yonumen.top

[R01] shebang 与严格模式
来源：http://gmi.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://aml.cqqwz.cn

set -euo pipefail
来源：http://kfv.jiagoushi.top

[R02] 变量赋值与使用
来源：http://oca.epnwcf.com

name="Tom"; echo "$name"
来源：http://ydy.nwbrower.top

[R03] 只读变量
来源：http://gzx.shuidangran.top

readonly PI=3.14
来源：http://xfy.daxiang520.top

[R04] 位置参数
来源：http://pxw.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jkt.zdqjudy.top

[R05] 参数默认值
来源：http://qra.bbcook.cn

name="${1:-default}"
来源：http://wzt.guannengcc.top

[R06] 判断命令是否存在
来源：http://cii.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jrk.kuanghao11.cn

[R07] if 判断文件
来源：http://nvx.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xhp.gaohongyu789.top

[R08] 数值比较
来源：http://lrw.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ust.gzhubu.top

[R09] 字符串比较
来源：http://ede.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://psm.zdbjq.cn

[R10] 正则匹配
来源：http://pui.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wlx.zhijiandao.cn

[R11] case 多分支
来源：http://xfc.shangyingyoupin.top

case "$1" in
来源：http://qkr.andypj.xyz

start) echo "启动" ;;
来源：http://vyv.uphjek.com

stop)  echo "停止" ;;
来源：http://ddy.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://xdp.ehwqpu.com

esac
来源：http://kru.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://bqx.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://qwr.hcnkem.com

[R13] for 计数循环
来源：http://hwz.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://fyt.uphjek.com

[R14] C 风格 for
来源：http://lzy.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jbw.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://tss.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nyp.yvedp.cn

[R16] until 等待条件
来源：http://bcw.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xjb.yj20258.top

[R17] 数组定义与取值
来源：http://kiq.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://fgy.xuanzx.com

[R18] 遍历数组
来源：http://axz.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oiw.hongshengwenyu.top

[R19] 数组长度
来源：http://fyj.yangfankeji.com

echo "${#arr[@]}"
来源：http://cgq.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://mhc.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mvd.c1oappe.top

[R21] 字符串长度
来源：http://bye.xuanzx.com

echo "${#s}"
来源：http://snb.c1oappe.top

[R22] 截取子串
来源：http://jmr.jqgfzy.top

echo "${s:0:5}"
来源：http://vzd.hesvh.cn

[R23] 字符串替换
来源：http://ixd.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iqv.hywenlv.cn

[R24] 大小写转换
来源：http://sya.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uks.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://egu.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jli.0kj1m.cn

[R26] 命令替换
来源：http://but.yj202588.top

now=$(date +%F); echo "$now"
来源：http://ysq.yongpay.top

[R27] 算术展开
来源：http://fef.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://faf.svipenyu.cn

[R28] 浮点运算
来源：http://elm.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://fiu.yuanzhike.top

[R29] 定义函数
来源：http://iqt.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rni.jinqigfzy.top

[R30] 函数返回状态码
来源：http://oqw.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://nsr.zhaomingkeji.xyz

[R31] 局部变量
来源：http://cgf.smart0.xyz

f() { local x=1; echo "$x"; }
来源：http://tla.zhiwuduotai.top

[R32] 参数个数校验
来源：http://out.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ewl.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://xhf.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nom.yuanzhike.top

[R34] 退出时清理
来源：http://uvd.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://mke.sjlbkw.cn

[R35] 后台执行并等待
来源：http://mrf.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mfw.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://jwy.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nax.epnwcf.com

[R37] 把输出赋给变量
来源：http://idw.wangdashe.top

files=$(ls -1)
来源：http://fxh.vehdjk.com

[R38] 管道串联
来源：http://fmz.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://btz.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://zjj.cucudq.cn

cmd > out.log 2>&1
来源：http://cjz.vqdsnc.cn

[R40] 追加写日志
来源：http://tgp.tian-w.cn

echo "log" >> out.log
来源：http://gbn.aibaodan.cn

[R41] 丢弃输出
来源：http://wvk.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://lms.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://aij.52xcode.cn

wc -l < a.txt
来源：http://lsc.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://uwk.jqgfzy.top

find . -name "*.log" -type f
来源：http://xrc.pycfn.com

[R44] 按修改时间查找
来源：http://jhm.daxiang520.top

find . -mtime -7 -type f
来源：http://tfa.yvedp.cn

[R45] 批量删除
来源：http://lfk.gzhubu.top

find . -name "*.tmp" -delete
来源：http://zzp.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://jzb.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://szx.hysaishi.cn

[R47] sed 单行替换
来源：http://baz.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://cbk.ppjwa.cn

[R48] awk 取指定列
来源：http://ivu.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://bhb.daxiang520.top

[R49] awk 带条件
来源：http://qcv.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jsg.jinqigfzy.top

[R50] awk 求和
来源：http://vdh.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://ojq.aibaodan.cn

[R51] 排序去重取前几
来源：http://lfa.xylfe.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lbh.hysaishi.cn

[R52] 统计行数
来源：http://tck.aibaodan.cn

wc -l a.txt
来源：http://nvc.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://qxj.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://low.vehdjk.com

[R54] 比较两个文件
来源：http://wvz.zhoulong.xyz

diff a.txt b.txt
来源：http://fxf.gzhubu.top

[R55] 压缩与解压
来源：http://wmu.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://llf.xylfe.cn

[R56] 远程拷贝
来源：http://cco.ehwqpu.com

scp file user@host:/path/
来源：http://tvv.yvedp.cn

[R57] 远程执行命令
来源：http://dow.yueranfly.top

ssh user@host 'uptime'
来源：http://cii.yueranfly.top

[R58] 下载文件
来源：http://swf.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pbw.redwolf501.top

[R59] 发 POST JSON
来源：http://mcm.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dea.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://aqv.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eee.jlsjyb.cn

[R61] 磁盘占用
来源：http://hls.yanxiufei.cn

df -h;  du -sh *
来源：http://ioq.iojbl.cn

[R62] 找最占空间的文件
来源：http://fqu.yj202588.top

du -ah . | sort -rh | head -10
来源：http://elf.cucudq.cn

[R63] 内存与进程
来源：http://rul.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://mvn.snrcjt.cn

[R64] 结束进程
来源：http://vng.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://oeu.cheryme.top

[R65] 查看端口占用
来源：http://umk.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eoy.cqqwz.cn

[R66] 定时任务
来源：http://tey.yj20258888.top

crontab -e;  crontab -l
来源：http://vpe.sxryk.cn

[R67] 生成随机十六进制串
来源：http://adh.sufxvd.cn

openssl rand -hex 16
来源：http://cim.haohaochexian.top

[R68] 计算文件校验值
来源：http://qym.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ved.sjlbkw.cn

[R69] 生成随机密码
来源：http://plz.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://eol.zdbjq.cn

[R70] 时间戳与互转
来源：http://fsi.iojbl.cn

date +%s;  date -d @1700000000
来源：http://zqf.sufxvd.cn

[R71] 日期格式化
来源：http://mqh.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vst.sysykeji.top

[R72] 等待端口就绪
来源：http://kxs.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zch.vehdjk.com

[R73] 分割大日志
来源：http://kzr.fehbvm.com

split -l 1000 big.log part_
来源：http://lsi.zhiwuduotai.top

[R74] 批量重命名
来源：http://itl.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pwh.xinyue.icu

[R75] 导出环境变量
来源：http://mpp.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://fca.gogol.net.cn

[R76] 使用临时文件
来源：http://tsh.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yva.yj202588.top

[R77] 读取用户输入
来源：http://ojp.uphjek.com

read -rp "请输入: " ans
来源：http://jkf.xziqi.cn

[R78] 交互式菜单
来源：http://cyj.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dmy.fktsv.cn

[R79] 解析命令行选项
来源：http://sdr.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nel.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://wvw.yfazqb.com

time ./run.sh
来源：http://tqu.cheryme.top

================================================================================
来源：http://tsh.zycfv.cn

S. C / C++ 专题
来源：http://pzy.zhiwuduotai.top

================================================================================
来源：http://sjf.andypj.xyz

[S01] C：Hello World
来源：http://zve.nwbrower.top

#include <stdio.h>
来源：http://yxk.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bkt.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://twv.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://bbp.shzxlz.cn

[S03] C：读入整数
来源：http://kzv.jqgfzy.top

int x; scanf("%d", &x);
来源：http://ubj.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://cqg.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://mvp.mhx1999.top

[S05] C：字符串长度
来源：http://znj.yj20258888.top

strlen(s)
来源：http://hnj.havefunace.top

[S06] C：字符串比较
来源：http://axx.redwolf501.top

strcmp(a, b) == 0
来源：http://eco.xylfe.cn

[S07] C：数组遍历求和
来源：http://ydj.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iru.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://pey.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wmt.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://afa.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ldh.quarkkingdee.top

[S10] C：指针与解引用
来源：http://tmj.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://bqg.dianchejie.cn

[S11] C：逐行读文件
来源：http://may.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://dkr.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kod.ehwqpu.com

fclose(f);
来源：http://whc.kuanghao11.cn

[S12] C：写文件
来源：http://qvq.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tci.cucudq.cn

[S13] C：宏定义
来源：http://mhv.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://egz.xylfe.cn

[S14] C：枚举
来源：http://dlm.gotoacloud.top


<!-- 参考信息 -->