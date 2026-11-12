代发 wailian999

[Q48] CTE 公用表表达式
来源：http://guw.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hvv.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://pmo.snrcjt.cn

[Q49] 更新单行
来源：http://rym.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dhg.birdmap.top

[Q50] 批量更新
来源：http://tix.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gzr.zhijiandao.cn

[Q51] 用子查询更新
来源：http://teu.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://alr.zhongyouzk.top

[Q52] 删除指定行
来源：http://lil.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://nou.chenzaomai.com

[Q53] 按条件删除
来源：http://ndr.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pna.fengsongda.top

[Q54] 清空表
来源：http://qpc.xziqi.cn

TRUNCATE TABLE logs;
来源：http://kvb.yj20258888.top

[Q55] 排名（并列占位）
来源：http://alt.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kee.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://pud.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://odo.birdmap.top

[Q57] 行号
来源：http://mqr.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wrs.epnwcf.com

[Q58] 累计求和
来源：http://atz.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pcj.hcnkem.com

[Q59] 分组内累计
来源：http://ore.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ocn.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://xuu.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gap.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zjx.nanxinkj.top

[Q61] 移动平均
来源：http://hhe.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://clu.jianghu66.top

[Q62] 分组占比
来源：http://big.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qba.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://elf.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://spk.quarkkingdee.top

[Q64] 提交事务
来源：http://aub.ydjk.org.cn

COMMIT;
来源：http://gjr.cucudq.cn

[Q65] 回滚事务
来源：http://khd.gogol.net.cn

ROLLBACK;
来源：http://gvo.guannengcc.top

[Q66] 行锁查询
来源：http://eas.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dch.vehdjk.com

[Q67] 设置隔离级别
来源：http://jlj.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xbb.gogol.net.cn

[Q68] 保存点
来源：http://sgc.sysykeji.top

SAVEPOINT sp1;
来源：http://nle.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://zer.guannengcc.top

[Q69] 查看执行计划
来源：http://dyo.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cko.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://ere.hesvh.cn

ANALYZE TABLE users;
来源：http://hqd.hcnkem.com

[Q71] 查看建表语句
来源：http://tqy.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bdt.havefunace.top

[Q72] 查看索引
来源：http://lsm.yanxiufei.cn

SHOW INDEX FROM users;
来源：http://pka.gzhubu.top

[Q73] 查看表状态
来源：http://kbl.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ytx.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://bhu.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qzl.cqqwz.cn

[Q75] 日期格式化
来源：http://bge.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fkt.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jgu.yueranfly.top

[Q76] 按天统计
来源：http://zam.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kcg.nanxinkj.top

[Q77] 时间加减
来源：http://wbf.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pcz.guannengcc.top

[Q78] 当前时间
来源：http://ooa.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ywa.dianchejie.cn

[Q79] 字符串拼接
来源：http://mvy.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vpg.mhx1999.top

[Q80] 字符串截取
来源：http://mek.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nrj.zhiwuduotai.top

[Q81] 字符串替换
来源：http://umd.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ubn.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://car.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uaj.ybcxt.top

[Q83] 大小写转换
来源：http://ofs.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qgd.yonumen.top

[Q84] 去除首尾空格
来源：http://voq.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://jpc.fengsongda.top

[Q85] 数值取整
来源：http://jik.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hat.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://qrl.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cqu.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://ant.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vdg.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://cyt.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://odh.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ouq.chenzaomai.com

[Q89] 判断表是否存在
来源：http://chr.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sui.mhx1999.top

[Q90] 生成序号列
来源：http://hcz.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hoi.yj20258.top

================================================================================
来源：http://gwt.c1oappe.top

R. Bash 专题
来源：http://ukt.shzxlz.cn

================================================================================
来源：http://ita.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://kku.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://ggt.pengpengdd.cyou

set -euo pipefail
来源：http://plr.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://jwy.daxiang520.top

name="Tom"; echo "$name"
来源：http://vjj.andypj.xyz

[R03] 只读变量
来源：http://cdd.jiagoushi.top

readonly PI=3.14
来源：http://wut.xuanzx.com

[R04] 位置参数
来源：http://kex.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bbu.vqdsnc.cn

[R05] 参数默认值
来源：http://ebn.hywenlv.cn

name="${1:-default}"
来源：http://owo.fehbvm.com

[R06] 判断命令是否存在
来源：http://nro.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tis.cucudq.cn

[R07] if 判断文件
来源：http://brm.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qdw.fktsv.cn

[R08] 数值比较
来源：http://vzf.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xtr.vqdsnc.cn

[R09] 字符串比较
来源：http://nmy.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://inn.jqgufenzy.top

[R10] 正则匹配
来源：http://iqo.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ibw.nwbrower.top

[R11] case 多分支
来源：http://rht.haohaochexian.top

case "$1" in
来源：http://aav.zhiwuduotai.top

start) echo "启动" ;;
来源：http://put.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://klf.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://dbk.gaohongyu789.top

esac
来源：http://xhd.ctjpmb.com

[R12] for 遍历文件
来源：http://cgp.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://zhu.yanxiufei.cn

[R13] for 计数循环
来源：http://zuk.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://jnm.epnwcf.com

[R14] C 风格 for
来源：http://thj.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qlr.vehdjk.com

[R15] while 逐行读文件
来源：http://jpg.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dme.ybcxt.top

[R16] until 等待条件
来源：http://fvl.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://djf.yuxming.cn

[R17] 数组定义与取值
来源：http://mxt.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://utm.hcnkem.com

[R18] 遍历数组
来源：http://tdt.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hyx.fehbvm.com

[R19] 数组长度
来源：http://uvd.jinqigufen.top

echo "${#arr[@]}"
来源：http://qdr.haohaochexian.top

[R20] 关联数组（字典）
来源：http://enn.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mbh.yuxming.cn

[R21] 字符串长度
来源：http://mvg.shangyingyoupin.top

echo "${#s}"
来源：http://asv.zdqjudy.top

[R22] 截取子串
来源：http://ltn.yongpay.top

echo "${s:0:5}"
来源：http://gey.xuanzx.com

[R23] 字符串替换
来源：http://euo.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ben.shangyingyoupin.top

[R24] 大小写转换
来源：http://pro.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://sfe.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://alx.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tmz.mhx1999.top

[R26] 命令替换
来源：http://afa.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://ljn.yvedp.cn

[R27] 算术展开
来源：http://ipr.fehbvm.com

echo $((1 + 2 * 3))
来源：http://eks.hysaishi.cn

[R28] 浮点运算
来源：http://quc.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://cjk.hesvh.cn

[R29] 定义函数
来源：http://mjp.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xch.yonumen.top

[R30] 函数返回状态码
来源：http://vnj.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://pne.hongshengwenyu.top

[R31] 局部变量
来源：http://ezw.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://hqb.zhoulong.xyz

[R32] 参数个数校验
来源：http://xmh.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ylq.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://kee.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rct.zhoulong.xyz

[R34] 退出时清理
来源：http://byz.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://pil.yuxming.cn

[R35] 后台执行并等待
来源：http://yur.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://sxr.fengsongda.top

[R36] 并发执行多个任务
来源：http://omw.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tqm.sufxvd.cn

[R37] 把输出赋给变量
来源：http://dcp.sweek.top

files=$(ls -1)
来源：http://jof.jinqigfzy.top

[R38] 管道串联
来源：http://xfg.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://emi.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://sdc.dashuyun.cn

cmd > out.log 2>&1
来源：http://fez.yj20258.top

[R40] 追加写日志
来源：http://qlb.sufxvd.cn

echo "log" >> out.log
来源：http://axf.andypj.xyz

[R41] 丢弃输出
来源：http://sln.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://ift.yvedp.cn

[R42] 输入重定向
来源：http://etv.meibo888.top

wc -l < a.txt
来源：http://lfm.zhongyouzk.top

[R43] 按名字查找文件
来源：http://xig.tanke756.top

find . -name "*.log" -type f
来源：http://izi.bjfxy.top

[R44] 按修改时间查找
来源：http://bry.c1oappe.top

find . -mtime -7 -type f
来源：http://lts.gogol.net.cn

[R45] 批量删除
来源：http://dwz.mhx1999.top

find . -name "*.tmp" -delete
来源：http://jad.wangdashe.top

[R46] 递归替换文件内容
来源：http://pob.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oah.xziqi.cn

[R47] sed 单行替换
来源：http://pqt.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://owl.xylfe.cn

[R48] awk 取指定列
来源：http://rph.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://sbk.fanxiaobao.xyz

[R49] awk 带条件
来源：http://pop.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rdm.fzhhl.top

[R50] awk 求和
来源：http://btm.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://iwr.birdmap.top

[R51] 排序去重取前几
来源：http://wll.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rat.quarkkingdee.top

[R52] 统计行数
来源：http://owj.haohaochexian.top

wc -l a.txt
来源：http://ekx.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://ewy.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lfn.tianlin.xyz

[R54] 比较两个文件
来源：http://prg.jlsjyb.cn

diff a.txt b.txt
来源：http://ykv.snrcjt.cn

[R55] 压缩与解压
来源：http://lhl.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jnh.sufxvd.cn

[R56] 远程拷贝
来源：http://vpd.yj20258888.top

scp file user@host:/path/
来源：http://gog.uphjek.com

[R57] 远程执行命令
来源：http://ugp.jiagoushi.top

ssh user@host 'uptime'
来源：http://xkl.wangshuangyany.cn

[R58] 下载文件
来源：http://tbv.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xmw.gaohongyu789.top

[R59] 发 POST JSON
来源：http://btv.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kvp.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://pof.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uvn.vqdsnc.cn

[R61] 磁盘占用
来源：http://xts.pycfn.com

df -h;  du -sh *
来源：http://erd.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://hfl.yonumen.top

du -ah . | sort -rh | head -10
来源：http://ixf.pycfn.com

[R63] 内存与进程
来源：http://jbb.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://bve.hcnkem.com

[R64] 结束进程
来源：http://cgs.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://bps.zhoulong.xyz

[R65] 查看端口占用
来源：http://klv.zhengqikj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://byf.kuanghao11.cn

[R66] 定时任务
来源：http://ino.cashguo.top

crontab -e;  crontab -l
来源：http://voj.hesvh.cn

[R67] 生成随机十六进制串
来源：http://xfd.redwolf501.top

openssl rand -hex 16
来源：http://idk.0kj1m.cn

[R68] 计算文件校验值
来源：http://xzs.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://wvi.meibo888.top

[R69] 生成随机密码
来源：http://idb.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://bjt.sysykeji.top

[R70] 时间戳与互转
来源：http://mzq.hesvh.cn

date +%s;  date -d @1700000000
来源：http://tie.chenzaomai.com

[R71] 日期格式化
来源：http://xki.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ccp.cqqwz.cn

[R72] 等待端口就绪
来源：http://kmo.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://luv.316326.xyz

[R73] 分割大日志
来源：http://byf.vqdsnc.cn

split -l 1000 big.log part_
来源：http://nfl.haohaochexian.top

[R74] 批量重命名
来源：http://yvj.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gfq.sxryk.cn

[R75] 导出环境变量
来源：http://aaf.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://vqo.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://snu.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rjw.cqqwz.cn

[R77] 读取用户输入
来源：http://yaz.hnxiangtu.top

read -rp "请输入: " ans
来源：http://rxg.andypj.xyz

[R78] 交互式菜单
来源：http://vhy.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hth.ydzc1.top

[R79] 解析命令行选项
来源：http://dqk.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dik.uphjek.com

[R80] 查看脚本执行耗时
来源：http://fco.guowangkeji.top

time ./run.sh
来源：http://opt.dashuyun.cn

================================================================================
来源：http://eeq.yuxming.cn

S. C / C++ 专题
来源：http://khr.jinqigfzy.top

================================================================================
来源：http://zbd.vehdjk.com

[S01] C：Hello World
来源：http://ilo.vehdjk.com

#include <stdio.h>
来源：http://ejr.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sca.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://zdj.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://alh.xuanzx.com

[S03] C：读入整数
来源：http://sch.cheryme.top

int x; scanf("%d", &x);
来源：http://yde.zhoulong.xyz

[S04] C：字符串复制
来源：http://lhu.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://jjw.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://xmh.ydzc1.top

strlen(s)
来源：http://whq.yuanzhike.top

[S06] C：字符串比较
来源：http://izg.zhongyouzk.top

strcmp(a, b) == 0
来源：http://kvy.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://ugu.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gwp.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://gzt.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://frc.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://zdh.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zat.sysykeji.top

[S10] C：指针与解引用
来源：http://xfc.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://oww.ivvv.top

[S11] C：逐行读文件
来源：http://rfj.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://lfz.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lld.dashuyun.cn

fclose(f);
来源：http://osy.yj202588.top

[S12] C：写文件
来源：http://jqi.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mes.sweek.top

[S13] C：宏定义
来源：http://pvb.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://thz.shangyingyoupin.top

[S14] C：枚举
来源：http://hfe.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://zod.shanyushiyangtech.top

[S15] C：类型转换
来源：http://nwc.zhengqikj.top

(double) a / b
来源：http://wwc.shzxlz.cn

[S16] C：位操作置位
来源：http://ceh.ehwqpu.com

x |= (1 << 3);
来源：http://rtb.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://odm.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://afy.quarkkingdee.top

[S18] C：命令行参数
来源：http://epz.52xcode.cn


<!-- 参考信息 -->