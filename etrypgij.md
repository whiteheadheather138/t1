代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xye.sysykeji.top

[Q52] 删除指定行
来源：http://yoe.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://ocv.52xcode.cn

[Q53] 按条件删除
来源：http://iff.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ujv.tianlin.xyz

[Q54] 清空表
来源：http://izr.yueranfly.top

TRUNCATE TABLE logs;
来源：http://cqe.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://eub.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pey.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://vem.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bvi.shanyushiyangkeji.top

[Q57] 行号
来源：http://lgu.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mgb.gaohongyu789.top

[Q58] 累计求和
来源：http://eas.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nkb.aizwys.cn

[Q59] 分组内累计
来源：http://oxx.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iba.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://xzy.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rpo.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wlz.daxiang520.top

[Q61] 移动平均
来源：http://ooe.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jxv.yj20258.top

[Q62] 分组占比
来源：http://jko.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wfc.yanxiufei.cn

[Q63] 开启事务
来源：http://qjw.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://rcq.xuetiantiany.cn

[Q64] 提交事务
来源：http://sjp.jinyuanbaomall.cn

COMMIT;
来源：http://jwt.cucudq.cn

[Q65] 回滚事务
来源：http://nsv.guannengcc.top

ROLLBACK;
来源：http://uwi.hnxiangtu.top

[Q66] 行锁查询
来源：http://aiq.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gwy.chenlongwang.top

[Q67] 设置隔离级别
来源：http://xre.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://urv.jyoumei.cn

[Q68] 保存点
来源：http://xfw.ybcxt.top

SAVEPOINT sp1;
来源：http://hah.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://adt.nanxuanxn.top

[Q69] 查看执行计划
来源：http://nef.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gas.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://ogq.cqqwz.cn

ANALYZE TABLE users;
来源：http://gnh.aibaodan.cn

[Q71] 查看建表语句
来源：http://dqs.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rfq.ctjpmb.com

[Q72] 查看索引
来源：http://pun.xziqi.cn

SHOW INDEX FROM users;
来源：http://lhq.svipenyu.cn

[Q73] 查看表状态
来源：http://ooz.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qjh.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://isj.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eby.aibaodan.cn

[Q75] 日期格式化
来源：http://esb.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xmb.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qdc.dashuyun.cn

[Q76] 按天统计
来源：http://zwd.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ogk.daria6918.cn

[Q77] 时间加减
来源：http://egd.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xqz.zhixingplan.top

[Q78] 当前时间
来源：http://rbp.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aax.xuanzx.com

[Q79] 字符串拼接
来源：http://wag.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://evm.fzhhl.top

[Q80] 字符串截取
来源：http://gdz.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gzl.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://osy.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vqz.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://nye.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bkg.nanxinkj.top

[Q83] 大小写转换
来源：http://gdz.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bah.birdmap.top

[Q84] 去除首尾空格
来源：http://cpe.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://lxy.cheryme.top

[Q85] 数值取整
来源：http://ddi.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dyt.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://znv.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://atz.c1oappe.top

[Q87] JSON 字段做条件
来源：http://zzd.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jdq.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://aez.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://itt.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iae.zdbjq.cn

[Q89] 判断表是否存在
来源：http://zsj.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://skb.dashuyun.cn

[Q90] 生成序号列
来源：http://ajz.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cpv.tianlin.xyz

================================================================================
来源：http://wgs.hcnkem.com

R. Bash 专题
来源：http://vsp.hcnkem.com

================================================================================
来源：http://ojd.cdnleiting.top

[R01] shebang 与严格模式
来源：http://nod.ehwqpu.com

#!/usr/bin/env bash
来源：http://lza.xingfuxueyuan.xyz

set -euo pipefail
来源：http://qqr.yj20258.top

[R02] 变量赋值与使用
来源：http://ooq.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://mrc.jiagoushi.top

[R03] 只读变量
来源：http://rni.zdqjudy.top

readonly PI=3.14
来源：http://vto.cashguo.top

[R04] 位置参数
来源：http://txj.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://grw.mhx1999.top

[R05] 参数默认值
来源：http://bqx.9152youxi.cn

name="${1:-default}"
来源：http://mtf.nanxinkj.top

[R06] 判断命令是否存在
来源：http://sxt.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lhw.cashguo.top

[R07] if 判断文件
来源：http://bai.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uyd.fanxiaobao.xyz

[R08] 数值比较
来源：http://tmq.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hdc.zdbjq.cn

[R09] 字符串比较
来源：http://fgl.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jeu.hcnkem.com

[R10] 正则匹配
来源：http://qsg.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zfq.quarkkingdee.top

[R11] case 多分支
来源：http://wsx.jlsjyb.cn

case "$1" in
来源：http://sfj.redwolf501.top

start) echo "启动" ;;
来源：http://iet.c1oappe.top

stop)  echo "停止" ;;
来源：http://bqs.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://soq.quarkkingdee.top

esac
来源：http://euc.andypj.xyz

[R12] for 遍历文件
来源：http://bqr.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://erz.guowangkeji.top

[R13] for 计数循环
来源：http://rll.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://ybi.sxryk.cn

[R14] C 风格 for
来源：http://phl.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kvo.zdbjq.cn

[R15] while 逐行读文件
来源：http://ihk.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdq.shuidangran.top

[R16] until 等待条件
来源：http://sry.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bkv.kuanghao11.cn

[R17] 数组定义与取值
来源：http://bbj.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qpc.vehdjk.com

[R18] 遍历数组
来源：http://mfp.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ncd.andypj.xyz

[R19] 数组长度
来源：http://pbl.hnxiangtu.top

echo "${#arr[@]}"
来源：http://tff.guowangkeji.top

[R20] 关联数组（字典）
来源：http://cos.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rok.yj202588.top

[R21] 字符串长度
来源：http://hhc.daria6918.cn

echo "${#s}"
来源：http://ieg.yangfankeji.com

[R22] 截取子串
来源：http://gal.yongpay.top

echo "${s:0:5}"
来源：http://kjt.kuanghao11.cn

[R23] 字符串替换
来源：http://rvm.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fpy.zhixingplan.top

[R24] 大小写转换
来源：http://qgz.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lcu.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://elb.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://kgd.hcnkem.com

[R26] 命令替换
来源：http://imm.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://flk.aibaodan.cn

[R27] 算术展开
来源：http://dah.316326.xyz

echo $((1 + 2 * 3))
来源：http://gfs.guowangkeji.top

[R28] 浮点运算
来源：http://hah.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://ykr.nwbrower.top

[R29] 定义函数
来源：http://scz.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rdo.yj20258.top

[R30] 函数返回状态码
来源：http://ays.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://cgw.hcnkem.com

[R31] 局部变量
来源：http://ezb.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://oei.andypj.xyz

[R32] 参数个数校验
来源：http://nni.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gxl.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://mhx.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kuk.bbcook.cn

[R34] 退出时清理
来源：http://arc.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://zbf.kuanghao11.cn

[R35] 后台执行并等待
来源：http://nvh.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ciu.aizwys.cn

[R36] 并发执行多个任务
来源：http://siw.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://glx.yangfankeji.com

[R37] 把输出赋给变量
来源：http://lee.xuanzx.com

files=$(ls -1)
来源：http://bhm.fktsv.cn

[R38] 管道串联
来源：http://soi.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://sws.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://puu.epnwcf.com

cmd > out.log 2>&1
来源：http://mwx.zhengqikj.top

[R40] 追加写日志
来源：http://gli.yanxiufei.cn

echo "log" >> out.log
来源：http://ype.quarkkingdee.top

[R41] 丢弃输出
来源：http://neq.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://ops.havefunace.top

[R42] 输入重定向
来源：http://yeu.bbcook.cn

wc -l < a.txt
来源：http://umf.ybcxt.top

[R43] 按名字查找文件
来源：http://tpl.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://vbb.aibaodan.cn

[R44] 按修改时间查找
来源：http://zaz.jyoumei.cn

find . -mtime -7 -type f
来源：http://yga.tianlin.xyz

[R45] 批量删除
来源：http://kct.xuanzx.com

find . -name "*.tmp" -delete
来源：http://nap.meibo888.top

[R46] 递归替换文件内容
来源：http://ymu.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uxr.fehbvm.com

[R47] sed 单行替换
来源：http://knb.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gff.ctjpmb.com

[R48] awk 取指定列
来源：http://gim.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://rte.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://fsw.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ulx.dianchejie.cn

[R50] awk 求和
来源：http://woq.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://vvo.chenzaomai.com

[R51] 排序去重取前几
来源：http://zqm.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://grn.hesvh.cn

[R52] 统计行数
来源：http://dxk.cdnleiting.top

wc -l a.txt
来源：http://qbi.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://chp.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lbr.redwolf501.top

[R54] 比较两个文件
来源：http://lhp.hesvh.cn

diff a.txt b.txt
来源：http://xtv.cucudq.cn

[R55] 压缩与解压
来源：http://fxw.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lvz.hesvh.cn

[R56] 远程拷贝
来源：http://qtd.fktsv.cn

scp file user@host:/path/
来源：http://yqj.kuanghao11.cn

[R57] 远程执行命令
来源：http://twc.kuanghao11.cn

ssh user@host 'uptime'
来源：http://jwq.kuanghao11.cn

[R58] 下载文件
来源：http://qbd.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ccq.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://bno.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dqu.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://acj.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hpy.yj20258.top

[R61] 磁盘占用
来源：http://gns.tian-w.cn

df -h;  du -sh *
来源：http://qpc.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://iod.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://knb.tanke756.top

[R63] 内存与进程
来源：http://gsv.tanke756.top

free -h;  ps aux | grep nginx
来源：http://hnv.zhijiandao.cn

[R64] 结束进程
来源：http://wdg.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://gmf.cqqwz.cn

[R65] 查看端口占用
来源：http://gyn.sysykeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkf.tianlin.xyz

[R66] 定时任务
来源：http://mpm.haohaochexian.top

crontab -e;  crontab -l
来源：http://rfp.xinyue.icu

[R67] 生成随机十六进制串
来源：http://nin.sweek.top

openssl rand -hex 16
来源：http://bwr.9152youxi.cn

[R68] 计算文件校验值
来源：http://hbq.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://duv.xuanzx.com

[R69] 生成随机密码
来源：http://pjf.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://syt.aizwys.cn

[R70] 时间戳与互转
来源：http://nfr.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://lyx.tanke756.top

[R71] 日期格式化
来源：http://mxt.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iiv.gzhubu.top

[R72] 等待端口就绪
来源：http://vft.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://prm.aizwys.cn

[R73] 分割大日志
来源：http://axn.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://vug.yonumen.top

[R74] 批量重命名
来源：http://jew.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hhx.ybcxt.top

[R75] 导出环境变量
来源：http://jxn.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://mdb.aizwys.cn

[R76] 使用临时文件
来源：http://jhl.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yoh.zhoulong.xyz

[R77] 读取用户输入
来源：http://kpj.ppjwa.cn

read -rp "请输入: " ans
来源：http://iwf.hammf.cn

[R78] 交互式菜单
来源：http://spj.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yjn.dianchejie.cn

[R79] 解析命令行选项
来源：http://asi.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dsr.yonumen.top

[R80] 查看脚本执行耗时
来源：http://ksj.shzxlz.cn

time ./run.sh
来源：http://gvz.jinghuilouyu.cn

================================================================================
来源：http://cjs.guannengcc.top

S. C / C++ 专题
来源：http://sef.hongshengwenyu.top

================================================================================
来源：http://yqc.yanxiufei.cn

[S01] C：Hello World
来源：http://mfy.bjfxy.top

#include <stdio.h>
来源：http://ndr.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jyg.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://shs.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://fhr.hcnkem.com

[S03] C：读入整数
来源：http://idu.shzxlz.cn

int x; scanf("%d", &x);
来源：http://tul.andypj.xyz

[S04] C：字符串复制
来源：http://bfn.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://vvq.nanxuanxn.top

[S05] C：字符串长度
来源：http://wbm.0kj1m.cn

strlen(s)
来源：http://lkp.fktsv.cn

[S06] C：字符串比较
来源：http://jit.fzhhl.top

strcmp(a, b) == 0
来源：http://cse.shuidangran.top

[S07] C：数组遍历求和
来源：http://enk.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nbd.316326.xyz

[S08] C：动态内存分配与释放
来源：http://bdf.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bqs.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://adz.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sag.jqgufenzy.top

[S10] C：指针与解引用
来源：http://emi.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://qzw.yj20258888.top

[S11] C：逐行读文件
来源：http://sca.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://hjn.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://ini.zhiwuduotai.top

fclose(f);
来源：http://xyq.guannengcc.top

[S12] C：写文件
来源：http://kpv.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://amx.fehbvm.com

[S13] C：宏定义
来源：http://rcy.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxi.redwolf501.top

[S14] C：枚举
来源：http://yeq.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://urm.kuanghao11.cn

[S15] C：类型转换
来源：http://cib.hnqzz.top

(double) a / b
来源：http://ksc.sufxvd.cn

[S16] C：位操作置位
来源：http://fck.0kj1m.cn

x |= (1 << 3);
来源：http://lbc.wangdashe.top

[S17] C：安全拼接字符串
来源：http://pgb.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mzc.mhx1999.top

[S18] C：命令行参数
来源：http://xrp.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://ris.gzhubu.top

[S19] C：快速排序
来源：http://uoc.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://bmi.hywenlv.cn

[S20] C：二分查找
来源：http://zvb.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ddj.bbcook.cn

[S21] C：字符类别判断
来源：http://mka.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mzu.fzhhl.top

[S22] C：字符串转数字
来源：http://iwh.ivvv.top


<!-- 参考信息 -->