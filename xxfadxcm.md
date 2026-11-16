代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rjg.yongpay.top

[Q52] 删除指定行
来源：http://jvu.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://pus.316326.xyz

[Q53] 按条件删除
来源：http://mde.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ves.jianghu66.top

[Q54] 清空表
来源：http://ile.xziqi.cn

TRUNCATE TABLE logs;
来源：http://zgo.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://ueb.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nbe.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://syr.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dhm.jinqigufen.top

[Q57] 行号
来源：http://pzv.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rud.yuanzhike.top

[Q58] 累计求和
来源：http://vbe.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://grn.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://iwy.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iyw.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://uwq.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mfa.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mtl.yanxiufei.cn

[Q61] 移动平均
来源：http://oba.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pwb.uphjek.com

[Q62] 分组占比
来源：http://zes.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nbc.aibaodan.cn

[Q63] 开启事务
来源：http://cao.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fhk.jqgufenzy.top

[Q64] 提交事务
来源：http://fja.zhaomingkeji.xyz

COMMIT;
来源：http://xop.jianghu66.top

[Q65] 回滚事务
来源：http://gjq.sufxvd.cn

ROLLBACK;
来源：http://cfa.zhijiandao.cn

[Q66] 行锁查询
来源：http://acu.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kvn.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://tzp.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ddm.jinqigufen.top

[Q68] 保存点
来源：http://cgd.yueranfly.top

SAVEPOINT sp1;
来源：http://pww.tarul.cn

ROLLBACK TO sp1;
来源：http://eox.ehwqpu.com

[Q69] 查看执行计划
来源：http://vsm.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://akn.cqqwz.cn

[Q70] 更新统计信息
来源：http://yrk.yueranfly.top

ANALYZE TABLE users;
来源：http://jxo.vqdsnc.cn

[Q71] 查看建表语句
来源：http://rix.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://exi.cqqwz.cn

[Q72] 查看索引
来源：http://aof.zycfv.cn

SHOW INDEX FROM users;
来源：http://idn.jianghu66.top

[Q73] 查看表状态
来源：http://udq.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wuw.0kj1m.cn

[Q74] 强制使用索引
来源：http://kcd.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ikm.pycfn.com

[Q75] 日期格式化
来源：http://ird.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ccy.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hif.uphjek.com

[Q76] 按天统计
来源：http://wul.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mpm.yj202588.top

[Q77] 时间加减
来源：http://rzq.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dvp.nwbrower.top

[Q78] 当前时间
来源：http://pdv.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vni.guowangkeji.top

[Q79] 字符串拼接
来源：http://ejm.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rsr.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://qea.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uqm.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://nkd.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wbw.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://nfr.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://udp.guannengcc.top

[Q83] 大小写转换
来源：http://gpo.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hya.yueranfly.top

[Q84] 去除首尾空格
来源：http://iqx.sweek.top

SELECT TRIM(name) FROM users;
来源：http://cge.yuxming.cn

[Q85] 数值取整
来源：http://odj.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ald.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://bix.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mqs.ybcxt.top

[Q87] JSON 字段做条件
来源：http://uwq.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bhu.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://pzj.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hhg.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ibw.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://hhh.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dnr.jqgufenzy.top

[Q90] 生成序号列
来源：http://fbx.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dkn.nwbrower.top

================================================================================
来源：http://puu.quarkkingdee.top

R. Bash 专题
来源：http://tpy.yfazqb.com

================================================================================
来源：http://mlz.sweek.top

[R01] shebang 与严格模式
来源：http://aam.fengsongda.top

#!/usr/bin/env bash
来源：http://onm.nanxuanxn.top

set -euo pipefail
来源：http://dgs.vehdjk.com

[R02] 变量赋值与使用
来源：http://sem.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://ejh.zhongyouzk.top

[R03] 只读变量
来源：http://jib.c1oappe.top

readonly PI=3.14
来源：http://utj.gogol.net.cn

[R04] 位置参数
来源：http://zak.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mri.zycfv.cn

[R05] 参数默认值
来源：http://tsj.daxiang520.top

name="${1:-default}"
来源：http://pms.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://hzq.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sgg.zhongyouzk.top

[R07] if 判断文件
来源：http://cug.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wsk.ivvv.top

[R08] 数值比较
来源：http://shq.zhaomingkeji.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://xvh.sysykeji.top

[R09] 字符串比较
来源：http://csc.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ywz.redwolf501.top

[R10] 正则匹配
来源：http://igl.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nid.316326.xyz

[R11] case 多分支
来源：http://ght.hfpthk.cn

case "$1" in
来源：http://iqy.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://zvh.yj20258.top

stop)  echo "停止" ;;
来源：http://fqd.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://irt.cqqwz.cn

esac
来源：http://upu.guannengcc.top

[R12] for 遍历文件
来源：http://giq.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://erc.havefunace.top

[R13] for 计数循环
来源：http://kap.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://unl.andypj.xyz

[R14] C 风格 for
来源：http://umd.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gfk.dashuyun.cn

[R15] while 逐行读文件
来源：http://rmu.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://urq.ydzc1.top

[R16] until 等待条件
来源：http://gyy.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bgy.wangdashe.top

[R17] 数组定义与取值
来源：http://giy.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://zfn.nwbrower.top

[R18] 遍历数组
来源：http://klt.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dkh.havefunace.top

[R19] 数组长度
来源：http://wgw.xinyue.icu

echo "${#arr[@]}"
来源：http://wgt.yuxming.cn

[R20] 关联数组（字典）
来源：http://ftz.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gdq.tarul.cn

[R21] 字符串长度
来源：http://qdt.jinghuilouyu.cn

echo "${#s}"
来源：http://wav.ppjwa.cn

[R22] 截取子串
来源：http://nnx.yj20258.top

echo "${s:0:5}"
来源：http://miv.hysaishi.cn

[R23] 字符串替换
来源：http://qhz.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://peo.ivvv.top

[R24] 大小写转换
来源：http://xmr.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kfm.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://jqh.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qct.hongshengwenyu.top

[R26] 命令替换
来源：http://wzs.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://cji.meibo888.top

[R27] 算术展开
来源：http://oga.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://hip.daria6918.cn

[R28] 浮点运算
来源：http://dzq.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://scg.jiagoushi.top

[R29] 定义函数
来源：http://hak.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nqm.hysaishi.cn

[R30] 函数返回状态码
来源：http://ygs.jyoumei.cn

f() { return 0; }; f || echo "失败了"
来源：http://jnx.tarul.cn

[R31] 局部变量
来源：http://sqf.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://fas.gogol.net.cn

[R32] 参数个数校验
来源：http://fhq.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sar.yongpay.top

[R33] 捕获错误并提示行号
来源：http://ivo.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sqt.haohaochexian.top

[R34] 退出时清理
来源：http://afu.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://ekp.316326.xyz

[R35] 后台执行并等待
来源：http://nei.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hxh.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://tvo.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yxn.xuanzx.com

[R37] 把输出赋给变量
来源：http://lzf.zhiwuduotai.top

files=$(ls -1)
来源：http://qzj.zhongyouzk.top

[R38] 管道串联
来源：http://xdw.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://avh.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://dve.yongpay.top

cmd > out.log 2>&1
来源：http://ktt.xinyue.icu

[R40] 追加写日志
来源：http://abn.yj20258.top

echo "log" >> out.log
来源：http://jkc.hywenlv.cn

[R41] 丢弃输出
来源：http://ruz.yfazqb.com

cmd >/dev/null 2>&1
来源：http://dcr.zdbjq.cn

[R42] 输入重定向
来源：http://ecy.fzhhl.top

wc -l < a.txt
来源：http://our.aizwys.cn

[R43] 按名字查找文件
来源：http://frh.ehwqpu.com

find . -name "*.log" -type f
来源：http://csk.gzhubu.top

[R44] 按修改时间查找
来源：http://jpq.jlsjyb.cn

find . -mtime -7 -type f
来源：http://gzy.shangyingyoupin.top

[R45] 批量删除
来源：http://fcc.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://rwz.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://pbp.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bxy.jiagoushi.top

[R47] sed 单行替换
来源：http://kzx.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://tad.yj20258.top

[R48] awk 取指定列
来源：http://teb.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://rpv.sjlbkw.cn

[R49] awk 带条件
来源：http://fsi.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://igv.haohaochexian.top

[R50] awk 求和
来源：http://oxm.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://jzm.sufxvd.cn

[R51] 排序去重取前几
来源：http://tzs.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kfj.vehdjk.com

[R52] 统计行数
来源：http://cxn.bjfxy.top

wc -l a.txt
来源：http://pxr.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://kcj.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wqq.shzxlz.cn

[R54] 比较两个文件
来源：http://fbr.aibaodan.cn

diff a.txt b.txt
来源：http://prx.ppjwa.cn

[R55] 压缩与解压
来源：http://bos.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ean.tianlin.xyz

[R56] 远程拷贝
来源：http://mch.havefunace.top

scp file user@host:/path/
来源：http://xiy.yonumen.top

[R57] 远程执行命令
来源：http://uiq.yvedp.cn

ssh user@host 'uptime'
来源：http://ejy.xinyue.icu

[R58] 下载文件
来源：http://agy.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pnz.jianghu66.top

[R59] 发 POST JSON
来源：http://cff.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://snl.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://cun.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qlx.jiagoushi.top

[R61] 磁盘占用
来源：http://fpv.snrcjt.cn

df -h;  du -sh *
来源：http://uhn.daxiang520.top

[R62] 找最占空间的文件
来源：http://zbk.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://ixc.yongpay.top

[R63] 内存与进程
来源：http://umd.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://plw.jyoumei.cn

[R64] 结束进程
来源：http://sxf.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://que.zhixingplan.top

[R65] 查看端口占用
来源：http://dnt.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mcz.nanxuanxn.top

[R66] 定时任务
来源：http://uni.mhx1999.top

crontab -e;  crontab -l
来源：http://btv.tarul.cn

[R67] 生成随机十六进制串
来源：http://ktp.gotoacloud.top

openssl rand -hex 16
来源：http://aqh.gaohongyu789.top

[R68] 计算文件校验值
来源：http://vjh.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mas.sysykeji.top

[R69] 生成随机密码
来源：http://hza.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://kqy.fzhhl.top

[R70] 时间戳与互转
来源：http://gpb.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://oha.316326.xyz

[R71] 日期格式化
来源：http://lyf.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xyi.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://ppo.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zmd.chenjidiqi.icu

[R73] 分割大日志
来源：http://tzd.sysykeji.top

split -l 1000 big.log part_
来源：http://yxf.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://gkx.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ybg.daxiang520.top

[R75] 导出环境变量
来源：http://tpc.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ckm.hnxiangtu.top

[R76] 使用临时文件
来源：http://rfg.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://efs.wangshuangyany.cn

[R77] 读取用户输入
来源：http://pid.nanxuanxn.top

read -rp "请输入: " ans
来源：http://yxp.52xcode.cn

[R78] 交互式菜单
来源：http://coz.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ftg.hnxiangtu.top

[R79] 解析命令行选项
来源：http://lgi.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qft.sweek.top

[R80] 查看脚本执行耗时
来源：http://zem.ppjwa.cn

time ./run.sh
来源：http://nhd.daria6918.cn

================================================================================
来源：http://tgb.zhengqikj.top

S. C / C++ 专题
来源：http://ozj.zhengqikj.top

================================================================================
来源：http://ins.c1oappe.top

[S01] C：Hello World
来源：http://aws.uphjek.com

#include <stdio.h>
来源：http://gpn.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ekl.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://fcl.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://jda.hcnkem.com

[S03] C：读入整数
来源：http://oku.jinqigufen.top

int x; scanf("%d", &x);
来源：http://dne.yonumen.top

[S04] C：字符串复制
来源：http://wlz.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://ngd.sjlbkw.cn

[S05] C：字符串长度
来源：http://ygb.aibaodan.cn

strlen(s)
来源：http://tov.wangshuangyany.cn

[S06] C：字符串比较
来源：http://pyq.shzxlz.cn

strcmp(a, b) == 0
来源：http://tai.daxiang520.top

[S07] C：数组遍历求和
来源：http://ydx.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://trl.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://twg.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hvs.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://vkw.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ovk.zhoulong.xyz

[S10] C：指针与解引用
来源：http://abl.52xcode.cn

int *p = &a;  *p = 5;
来源：http://wxs.xinyue.icu

[S11] C：逐行读文件
来源：http://lsu.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://rck.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://osc.guowangkeji.top

fclose(f);
来源：http://fkm.zhengqikj.top

[S12] C：写文件
来源：http://ini.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zmh.guannengcc.top

[S13] C：宏定义
来源：http://glp.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jan.iojbl.cn

[S14] C：枚举
来源：http://avc.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://apc.hongshengwenyu.top

[S15] C：类型转换
来源：http://duf.hywenlv.cn

(double) a / b
来源：http://jxx.ivvv.top

[S16] C：位操作置位
来源：http://eqp.hnqzz.top

x |= (1 << 3);
来源：http://oii.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://uoe.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://idu.0kj1m.cn

[S18] C：命令行参数
来源：http://umv.jinqigfzy.top

int main(int argc, char **argv)
来源：http://wfr.gzhubu.top

[S19] C：快速排序
来源：http://qfg.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://lpv.dianchejie.cn

[S20] C：二分查找
来源：http://bsk.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bjk.hywenlv.cn

[S21] C：字符类别判断
来源：http://opc.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jhp.cdnleiting.top

[S22] C：字符串转数字
来源：http://wod.ctjpmb.com


<!-- 参考信息 -->