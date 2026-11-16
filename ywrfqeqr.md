代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eiw.pycfn.com

[Q50] 批量更新
来源：http://pba.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fry.zdqjudy.top

[Q51] 用子查询更新
来源：http://cam.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pje.sweek.top

[Q52] 删除指定行
来源：http://buh.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://euj.52xcode.cn

[Q53] 按条件删除
来源：http://zvc.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lcp.havefunace.top

[Q54] 清空表
来源：http://low.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://aza.hesvh.cn

[Q55] 排名（并列占位）
来源：http://imo.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zel.redwolf501.top

[Q56] 密集排名（并列不占位）
来源：http://tjo.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dds.smart0.xyz

[Q57] 行号
来源：http://aoz.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bov.jlsjyb.cn

[Q58] 累计求和
来源：http://yln.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oer.fengsongda.top

[Q59] 分组内累计
来源：http://zgw.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tgg.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://rcs.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kpu.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ken.meibo888.top

[Q61] 移动平均
来源：http://raf.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://opv.hywenlv.cn

[Q62] 分组占比
来源：http://nom.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lex.ydzc1.top

[Q63] 开启事务
来源：http://nbe.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nqx.vehdjk.com

[Q64] 提交事务
来源：http://cye.ydjk.org.cn

COMMIT;
来源：http://zrx.fzhhl.top

[Q65] 回滚事务
来源：http://aef.meibo888.top

ROLLBACK;
来源：http://huz.hammf.cn

[Q66] 行锁查询
来源：http://ktp.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wzy.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://zbm.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bbu.cheryme.top

[Q68] 保存点
来源：http://sdp.gotoacloud.top

SAVEPOINT sp1;
来源：http://edw.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://bis.sufxvd.cn

[Q69] 查看执行计划
来源：http://ytg.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hak.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://xvp.fengsongda.top

ANALYZE TABLE users;
来源：http://qyd.ivvv.top

[Q71] 查看建表语句
来源：http://lmp.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wbx.yonumen.top

[Q72] 查看索引
来源：http://axg.aibaodan.cn

SHOW INDEX FROM users;
来源：http://zoz.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://kxb.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gwh.gaohongyu789.top

[Q74] 强制使用索引
来源：http://udp.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zit.chenjidiqi.icu

[Q75] 日期格式化
来源：http://ncz.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lfo.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bqd.9152youxi.cn

[Q76] 按天统计
来源：http://fmf.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://akw.hfpthk.cn

[Q77] 时间加减
来源：http://dmm.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pae.gzhubu.top

[Q78] 当前时间
来源：http://oon.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://unn.shuidangran.top

[Q79] 字符串拼接
来源：http://zjm.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gzw.hesvh.cn

[Q80] 字符串截取
来源：http://sgq.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://thy.dianchejie.cn

[Q81] 字符串替换
来源：http://kti.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wat.cheryme.top

[Q82] 字符长度与字节长度
来源：http://zok.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ehj.pengpengdd.cyou

[Q83] 大小写转换
来源：http://xmr.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pbu.jyoumei.cn

[Q84] 去除首尾空格
来源：http://jbj.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://ody.nwbrower.top

[Q85] 数值取整
来源：http://qyk.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wrr.pycfn.com

[Q86] 读取 JSON 字段
来源：http://oze.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uug.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://bro.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://isl.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://opg.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pbh.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wwv.nwbrower.top

[Q89] 判断表是否存在
来源：http://twe.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wmu.gotoacloud.top

[Q90] 生成序号列
来源：http://ziw.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vvk.9152youxi.cn

================================================================================
来源：http://nhb.jqgufenzy.top

R. Bash 专题
来源：http://zvi.hysaishi.cn

================================================================================
来源：http://iii.shuidangran.top

[R01] shebang 与严格模式
来源：http://lrb.ydjk.org.cn

#!/usr/bin/env bash
来源：http://oia.guowangkeji.top

set -euo pipefail
来源：http://xyv.uphjek.com

[R02] 变量赋值与使用
来源：http://vrp.vehdjk.com

name="Tom"; echo "$name"
来源：http://mps.nanxinkj.top

[R03] 只读变量
来源：http://xxm.hongshengwenyu.top

readonly PI=3.14
来源：http://byq.hnqzz.top

[R04] 位置参数
来源：http://fbm.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vwq.meibo888.top

[R05] 参数默认值
来源：http://vwy.nanxinkj.top

name="${1:-default}"
来源：http://tbc.cqqwz.cn

[R06] 判断命令是否存在
来源：http://nlm.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hcb.hnxiangtu.top

[R07] if 判断文件
来源：http://dzl.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zzu.zhaomingkeji.xyz

[R08] 数值比较
来源：http://xrr.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bcw.shuidangran.top

[R09] 字符串比较
来源：http://qwe.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tuk.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://ddu.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://swn.daria6918.cn

[R11] case 多分支
来源：http://htm.ydzc1.top

case "$1" in
来源：http://hqf.yj20258888.top

start) echo "启动" ;;
来源：http://fyk.cucudq.cn

stop)  echo "停止" ;;
来源：http://oog.wangdashe.top

*)     echo "未知命令" ;;
来源：http://llw.hywenlv.cn

esac
来源：http://tzc.yj20258888.top

[R12] for 遍历文件
来源：http://dqn.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://qmx.dianchejie.cn

[R13] for 计数循环
来源：http://qpg.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://xbm.vehdjk.com

[R14] C 风格 for
来源：http://pby.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://utn.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://axd.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iri.jiagoushi.top

[R16] until 等待条件
来源：http://jrn.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vlm.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://crb.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nsy.xziqi.cn

[R18] 遍历数组
来源：http://qzt.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kga.tianlin.xyz

[R19] 数组长度
来源：http://jnu.tarul.cn

echo "${#arr[@]}"
来源：http://cvk.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://edc.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vco.sysykeji.top

[R21] 字符串长度
来源：http://hyl.aizwys.cn

echo "${#s}"
来源：http://mrb.hammf.cn

[R22] 截取子串
来源：http://giu.cqqwz.cn

echo "${s:0:5}"
来源：http://ztw.hysaishi.cn

[R23] 字符串替换
来源：http://jsb.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qhm.quarkkingdee.top

[R24] 大小写转换
来源：http://pco.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fao.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://dke.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cwf.yonumen.top

[R26] 命令替换
来源：http://fvz.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://ujx.quarkkingdee.top

[R27] 算术展开
来源：http://dza.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://yyb.zhixingplan.top

[R28] 浮点运算
来源：http://usj.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://czl.gogol.net.cn

[R29] 定义函数
来源：http://rle.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jye.iojbl.cn

[R30] 函数返回状态码
来源：http://hdv.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://esh.jlsjyb.cn

[R31] 局部变量
来源：http://kpv.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://xxw.andypj.xyz

[R32] 参数个数校验
来源：http://vvh.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://biq.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://rmn.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zpi.haohaochexian.top

[R34] 退出时清理
来源：http://uhf.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://tiw.dianchejie.cn

[R35] 后台执行并等待
来源：http://yvb.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qky.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://wrf.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nzx.tanke756.top

[R37] 把输出赋给变量
来源：http://xqw.zdbjq.cn

files=$(ls -1)
来源：http://fhh.hnqzz.top

[R38] 管道串联
来源：http://ykc.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://pny.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://jae.uphjek.com

cmd > out.log 2>&1
来源：http://okn.yj20258888.top

[R40] 追加写日志
来源：http://yfa.cashguo.top

echo "log" >> out.log
来源：http://vvs.daxiang520.top

[R41] 丢弃输出
来源：http://isa.sxryk.cn

cmd >/dev/null 2>&1
来源：http://zhe.yj202588.top

[R42] 输入重定向
来源：http://bvi.shzxlz.cn

wc -l < a.txt
来源：http://klv.vehdjk.com

[R43] 按名字查找文件
来源：http://urb.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://xeq.ivvv.top

[R44] 按修改时间查找
来源：http://gaz.yangfankeji.com

find . -mtime -7 -type f
来源：http://yod.yfazqb.com

[R45] 批量删除
来源：http://baa.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://yen.yangfankeji.com

[R46] 递归替换文件内容
来源：http://slc.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gou.hnqzz.top

[R47] sed 单行替换
来源：http://jpm.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://zds.c1oappe.top

[R48] awk 取指定列
来源：http://ada.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://ypr.vehdjk.com

[R49] awk 带条件
来源：http://gco.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xfk.snrcjt.cn

[R50] awk 求和
来源：http://gnl.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rvw.jinqigfzy.top

[R51] 排序去重取前几
来源：http://yvh.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hok.daria6918.cn

[R52] 统计行数
来源：http://nao.pengpengdd.cyou

wc -l a.txt
来源：http://ctr.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://fkw.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ind.ydjk.org.cn

[R54] 比较两个文件
来源：http://drl.ivvv.top

diff a.txt b.txt
来源：http://mlh.nanxuanxn.top

[R55] 压缩与解压
来源：http://gbi.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dpx.sjlbkw.cn

[R56] 远程拷贝
来源：http://pwm.ybcxt.top

scp file user@host:/path/
来源：http://vvj.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://gza.jlsjyb.cn

ssh user@host 'uptime'
来源：http://rka.ppjwa.cn

[R58] 下载文件
来源：http://ckb.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rnd.zhengqikj.top

[R59] 发 POST JSON
来源：http://jel.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wrw.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://zie.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://orm.chenjidiqi.icu

[R61] 磁盘占用
来源：http://jju.316326.xyz

df -h;  du -sh *
来源：http://knu.zdbjq.cn

[R62] 找最占空间的文件
来源：http://iof.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://mro.guannengcc.top

[R63] 内存与进程
来源：http://gey.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://zhg.cashguo.top

[R64] 结束进程
来源：http://xwo.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://llz.zhijiandao.cn

[R65] 查看端口占用
来源：http://pin.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://izs.shangyingyoupin.top

[R66] 定时任务
来源：http://tqv.yuanzhike.top

crontab -e;  crontab -l
来源：http://wxx.redwolf501.top

[R67] 生成随机十六进制串
来源：http://bgt.havefunace.top

openssl rand -hex 16
来源：http://vnd.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://llu.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://gps.cucudq.cn

[R69] 生成随机密码
来源：http://stp.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://hon.sxryk.cn

[R70] 时间戳与互转
来源：http://lxd.fktsv.cn

date +%s;  date -d @1700000000
来源：http://axp.xinyue.icu

[R71] 日期格式化
来源：http://rsx.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nvr.snrcjt.cn

[R72] 等待端口就绪
来源：http://gsl.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yjs.tarul.cn

[R73] 分割大日志
来源：http://rpy.bjfxy.top

split -l 1000 big.log part_
来源：http://ivz.cashguo.top

[R74] 批量重命名
来源：http://xre.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aor.meibo888.top

[R75] 导出环境变量
来源：http://zef.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://kxe.9152youxi.cn

[R76] 使用临时文件
来源：http://iku.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://myo.sxryk.cn

[R77] 读取用户输入
来源：http://cmd.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://wpj.guowangkeji.top

[R78] 交互式菜单
来源：http://nrg.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xnt.vqdsnc.cn

[R79] 解析命令行选项
来源：http://aop.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iep.hcnkem.com

[R80] 查看脚本执行耗时
来源：http://lzo.xingfuxueyuan.xyz

time ./run.sh
来源：http://xwq.316326.xyz

================================================================================
来源：http://xwn.bjfxy.top

S. C / C++ 专题
来源：http://icr.wangdashe.top

================================================================================
来源：http://njb.nwbrower.top

[S01] C：Hello World
来源：http://gtl.ydjk.org.cn

#include <stdio.h>
来源：http://wmu.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://uvr.yj202588.top

[S02] C：变量与格式化输出
来源：http://nco.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://bcn.shuidangran.top

[S03] C：读入整数
来源：http://etm.yonumen.top

int x; scanf("%d", &x);
来源：http://mge.vqdsnc.cn

[S04] C：字符串复制
来源：http://ryf.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://dbl.nwbrower.top

[S05] C：字符串长度
来源：http://zrq.shanyushiyangkeji.top

strlen(s)
来源：http://swf.dashuyun.cn

[S06] C：字符串比较
来源：http://efx.tanke756.top

strcmp(a, b) == 0
来源：http://spx.aibaodan.cn

[S07] C：数组遍历求和
来源：http://hiu.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yvl.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://txz.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://taf.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://eyj.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jin.daxiang520.top

[S10] C：指针与解引用
来源：http://cmu.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://niv.zycfv.cn

[S11] C：逐行读文件
来源：http://uxm.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://cge.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://cjt.daria6918.cn

fclose(f);
来源：http://fwm.kuanghao11.cn

[S12] C：写文件
来源：http://lrj.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://csk.gzhubu.top

[S13] C：宏定义
来源：http://wjv.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dnr.haohaochexian.top

[S14] C：枚举
来源：http://sku.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://acw.hongshengwenyu.top

[S15] C：类型转换
来源：http://kyw.yonumen.top

(double) a / b
来源：http://qgb.zhixingplan.top

[S16] C：位操作置位
来源：http://xnx.fanxiaobao.xyz

x |= (1 << 3);
来源：http://vmw.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://cgc.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cas.shzxlz.cn

[S18] C：命令行参数
来源：http://lwo.cucudq.cn

int main(int argc, char **argv)
来源：http://fwy.xuanzx.com

[S19] C：快速排序
来源：http://ozv.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://okg.haohaochexian.top

[S20] C：二分查找
来源：http://vly.svipenyu.cn


<!-- 参考信息 -->