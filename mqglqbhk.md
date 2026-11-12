代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fyl.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://zln.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lri.ywan-chungtsiang.top

[Q57] 行号
来源：http://syr.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eri.uphjek.com

[Q58] 累计求和
来源：http://drr.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxf.smart0.xyz

[Q59] 分组内累计
来源：http://fbj.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cck.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://oag.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tlb.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qqk.kuanghao11.cn

[Q61] 移动平均
来源：http://sws.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kxg.guannengcc.top

[Q62] 分组占比
来源：http://iqj.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dae.0kj1m.cn

[Q63] 开启事务
来源：http://ohq.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://kqb.jqgufenzy.top

[Q64] 提交事务
来源：http://qer.fzhhl.top

COMMIT;
来源：http://ywz.yj20258888.top

[Q65] 回滚事务
来源：http://qnr.yanxiufei.cn

ROLLBACK;
来源：http://nkd.tanke756.top

[Q66] 行锁查询
来源：http://epk.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://svs.aibaodan.cn

[Q67] 设置隔离级别
来源：http://sup.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rpm.sysykeji.top

[Q68] 保存点
来源：http://ooj.zhoulong.xyz

SAVEPOINT sp1;
来源：http://hgj.ydzc1.top

ROLLBACK TO sp1;
来源：http://cno.hysaishi.cn

[Q69] 查看执行计划
来源：http://vqe.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ubn.yueranfly.top

[Q70] 更新统计信息
来源：http://blm.yuxming.cn

ANALYZE TABLE users;
来源：http://nzu.jyoumei.cn

[Q71] 查看建表语句
来源：http://ayw.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lcw.guowangkeji.top

[Q72] 查看索引
来源：http://oer.svipenyu.cn

SHOW INDEX FROM users;
来源：http://ojh.nanxinkj.top

[Q73] 查看表状态
来源：http://xms.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ksv.nanxinkj.top

[Q74] 强制使用索引
来源：http://pox.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bik.jianghu66.top

[Q75] 日期格式化
来源：http://oxm.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zts.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ckb.fanxiaobao.xyz

[Q76] 按天统计
来源：http://igy.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dbn.smart0.xyz

[Q77] 时间加减
来源：http://pvs.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mpd.gotoacloud.top

[Q78] 当前时间
来源：http://mwx.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cbo.tian-w.cn

[Q79] 字符串拼接
来源：http://amz.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ujg.gogol.net.cn

[Q80] 字符串截取
来源：http://wpv.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rph.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://ehk.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dhs.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://foi.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nhj.yangfankeji.com

[Q83] 大小写转换
来源：http://lmx.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dgg.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://jlc.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://pxx.pycfn.com

[Q85] 数值取整
来源：http://wrl.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wni.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://vzg.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ush.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://fwl.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ole.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://cjd.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kex.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vtw.hcnkem.com

[Q89] 判断表是否存在
来源：http://olq.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://geb.0kj1m.cn

[Q90] 生成序号列
来源：http://vay.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qfp.cucudq.cn

================================================================================
来源：http://csv.fehbvm.com

R. Bash 专题
来源：http://pjg.epnwcf.com

================================================================================
来源：http://zbz.guannengcc.top

[R01] shebang 与严格模式
来源：http://wsd.ctjpmb.com

#!/usr/bin/env bash
来源：http://rda.fanxiaobao.xyz

set -euo pipefail
来源：http://nje.xziqi.cn

[R02] 变量赋值与使用
来源：http://meg.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://awp.shangyingyoupin.top

[R03] 只读变量
来源：http://nbg.sxryk.cn

readonly PI=3.14
来源：http://oqb.pycfn.com

[R04] 位置参数
来源：http://kfa.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tes.gotoacloud.top

[R05] 参数默认值
来源：http://hmy.jqgufenzy.top

name="${1:-default}"
来源：http://mdo.gotoacloud.top

[R06] 判断命令是否存在
来源：http://dww.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oqp.cashguo.top

[R07] if 判断文件
来源：http://qzq.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxf.hysaishi.cn

[R08] 数值比较
来源：http://mri.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dpr.zdqjudy.top

[R09] 字符串比较
来源：http://vpa.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nwd.pycfn.com

[R10] 正则匹配
来源：http://quq.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ysh.ivvv.top

[R11] case 多分支
来源：http://knm.ctjpmb.com

case "$1" in
来源：http://kbb.9152youxi.cn

start) echo "启动" ;;
来源：http://ead.cucudq.cn

stop)  echo "停止" ;;
来源：http://nok.aibaodan.cn

*)     echo "未知命令" ;;
来源：http://xmc.gogol.net.cn

esac
来源：http://vre.fktsv.cn

[R12] for 遍历文件
来源：http://bov.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://qeg.wangshuangyany.cn

[R13] for 计数循环
来源：http://jxt.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://vei.gaohongyu789.top

[R14] C 风格 for
来源：http://ahu.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ybo.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://gys.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dzi.fktsv.cn

[R16] until 等待条件
来源：http://xlj.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://alj.ydjk.org.cn

[R17] 数组定义与取值
来源：http://qhs.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cpx.meibo888.top

[R18] 遍历数组
来源：http://rig.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gff.gotoacloud.top

[R19] 数组长度
来源：http://sgt.cucudq.cn

echo "${#arr[@]}"
来源：http://pya.hesvh.cn

[R20] 关联数组（字典）
来源：http://swh.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ewu.0kj1m.cn

[R21] 字符串长度
来源：http://obi.xuetiantiany.cn

echo "${#s}"
来源：http://pmp.ydzc1.top

[R22] 截取子串
来源：http://mge.zhixingplan.top

echo "${s:0:5}"
来源：http://lgi.havefunace.top

[R23] 字符串替换
来源：http://fgm.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wde.shzxlz.cn

[R24] 大小写转换
来源：http://avh.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://ltv.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://nzh.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jze.zdqjudy.top

[R26] 命令替换
来源：http://xrr.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://sqk.mhx1999.top

[R27] 算术展开
来源：http://kod.sxryk.cn

echo $((1 + 2 * 3))
来源：http://kat.yueranfly.top

[R28] 浮点运算
来源：http://alo.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://tja.hesvh.cn

[R29] 定义函数
来源：http://pif.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://crn.0kj1m.cn

[R30] 函数返回状态码
来源：http://qbu.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://nou.52xcode.cn

[R31] 局部变量
来源：http://fph.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://tjt.mhx1999.top

[R32] 参数个数校验
来源：http://hcf.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://anv.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://vdi.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wrm.tarul.cn

[R34] 退出时清理
来源：http://fuy.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://one.yfazqb.com

[R35] 后台执行并等待
来源：http://xul.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vzq.hcnkem.com

[R36] 并发执行多个任务
来源：http://xxc.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gsu.guannengcc.top

[R37] 把输出赋给变量
来源：http://myk.quarkkingdee.top

files=$(ls -1)
来源：http://wod.ctjpmb.com

[R38] 管道串联
来源：http://eye.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://dvt.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://tpa.jinqigufen.top

cmd > out.log 2>&1
来源：http://bcg.ydjk.org.cn

[R40] 追加写日志
来源：http://tvd.52xcode.cn

echo "log" >> out.log
来源：http://ovc.316326.xyz

[R41] 丢弃输出
来源：http://jub.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://sho.cucudq.cn

[R42] 输入重定向
来源：http://dxv.ivvv.top

wc -l < a.txt
来源：http://ala.yonumen.top

[R43] 按名字查找文件
来源：http://kyb.cheryme.top

find . -name "*.log" -type f
来源：http://mbj.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://jon.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://scg.hongshengwenyu.top

[R45] 批量删除
来源：http://csf.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://hdg.fktsv.cn

[R46] 递归替换文件内容
来源：http://ecl.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ody.yangfankeji.com

[R47] sed 单行替换
来源：http://jnz.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://zvx.nwbrower.top

[R48] awk 取指定列
来源：http://tbr.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://kfx.hysaishi.cn

[R49] awk 带条件
来源：http://zwy.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bvx.hnxiangtu.top

[R50] awk 求和
来源：http://yqr.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://bon.nanxinkj.top

[R51] 排序去重取前几
来源：http://kaq.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hkn.zhijiandao.cn

[R52] 统计行数
来源：http://qgq.gzhubu.top

wc -l a.txt
来源：http://qvs.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://soq.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nuq.nwbrower.top

[R54] 比较两个文件
来源：http://ffe.chenjidiqi.icu

diff a.txt b.txt
来源：http://ujc.gogol.net.cn

[R55] 压缩与解压
来源：http://bzh.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ywr.fktsv.cn

[R56] 远程拷贝
来源：http://mqn.ybcxt.top

scp file user@host:/path/
来源：http://zpq.pycfn.com

[R57] 远程执行命令
来源：http://ves.snrcjt.cn

ssh user@host 'uptime'
来源：http://uls.9152youxi.cn

[R58] 下载文件
来源：http://ccw.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cke.dianchejie.cn

[R59] 发 POST JSON
来源：http://qpu.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vzv.quarkkingdee.top

[R60] 只看 HTTP 状态码
来源：http://hfp.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://spn.fktsv.cn

[R61] 磁盘占用
来源：http://wvg.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://pbn.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://owt.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://frr.sxryk.cn

[R63] 内存与进程
来源：http://irr.uphjek.com

free -h;  ps aux | grep nginx
来源：http://jxi.jianghu66.top

[R64] 结束进程
来源：http://hof.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://qqp.0kj1m.cn

[R65] 查看端口占用
来源：http://pow.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xky.daxiang520.top

[R66] 定时任务
来源：http://hva.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://arm.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://hqm.ivvv.top

openssl rand -hex 16
来源：http://hfn.vqdsnc.cn

[R68] 计算文件校验值
来源：http://vdu.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://orp.andypj.xyz

[R69] 生成随机密码
来源：http://sgf.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://bvy.fktsv.cn

[R70] 时间戳与互转
来源：http://ijt.redwolf501.top

date +%s;  date -d @1700000000
来源：http://jpb.daria6918.cn

[R71] 日期格式化
来源：http://qaq.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://spq.guannengcc.top

[R72] 等待端口就绪
来源：http://tbz.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://usr.bbcook.cn

[R73] 分割大日志
来源：http://xmj.hcnkem.com

split -l 1000 big.log part_
来源：http://rod.meibo888.top

[R74] 批量重命名
来源：http://osn.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kna.52xcode.cn

[R75] 导出环境变量
来源：http://ztq.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://sxy.ydzc1.top

[R76] 使用临时文件
来源：http://hjj.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ajc.aizwys.cn

[R77] 读取用户输入
来源：http://bos.yuanzhike.top

read -rp "请输入: " ans
来源：http://jgq.zhijiandao.cn

[R78] 交互式菜单
来源：http://wvf.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kwu.svipenyu.cn

[R79] 解析命令行选项
来源：http://cpu.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rjw.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://vwh.chenlongwang.top

time ./run.sh
来源：http://drl.zdbjq.cn

================================================================================
来源：http://blt.yongpay.top

S. C / C++ 专题
来源：http://ode.cheryme.top

================================================================================
来源：http://kvw.smart0.xyz

[S01] C：Hello World
来源：http://vsk.kuanghao11.cn

#include <stdio.h>
来源：http://cbs.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hyv.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://gqt.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://uas.xuetiantiany.cn

[S03] C：读入整数
来源：http://ank.yuanzhike.top

int x; scanf("%d", &x);
来源：http://phl.gzhubu.top

[S04] C：字符串复制
来源：http://erb.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://vfy.ivvv.top

[S05] C：字符串长度
来源：http://myq.bjfxy.top

strlen(s)
来源：http://fyi.hfpthk.cn

[S06] C：字符串比较
来源：http://vvc.9152youxi.cn

strcmp(a, b) == 0
来源：http://yzy.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://dph.yj202588.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lez.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://uyo.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dko.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://xhp.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kvk.gaohongyu789.top

[S10] C：指针与解引用
来源：http://tpe.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://nep.sweek.top

[S11] C：逐行读文件
来源：http://wxe.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://ijg.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://smk.yvedp.cn

fclose(f);
来源：http://dwg.sxryk.cn

[S12] C：写文件
来源：http://szd.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hwq.gogol.net.cn

[S13] C：宏定义
来源：http://oip.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://chp.gotoacloud.top

[S14] C：枚举
来源：http://mmw.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://fqf.yj202588.top

[S15] C：类型转换
来源：http://xvf.nanxuanxn.top

(double) a / b
来源：http://tpo.redwolf501.top

[S16] C：位操作置位
来源：http://smz.52xcode.cn

x |= (1 << 3);
来源：http://emq.daxiang520.top

[S17] C：安全拼接字符串
来源：http://xpm.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xne.ybcxt.top

[S18] C：命令行参数
来源：http://elv.xinyue.icu

int main(int argc, char **argv)
来源：http://cvu.yj202588.top

[S19] C：快速排序
来源：http://ors.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://mkv.xuanzx.com

[S20] C：二分查找
来源：http://dhh.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jqe.ppjwa.cn

[S21] C：字符类别判断
来源：http://gap.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qdd.xylfe.cn

[S22] C：字符串转数字
来源：http://iml.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://pkt.yuanzhike.top

[S23] C：随机数
来源：http://ltk.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qpg.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://hho.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xok.tarul.cn

[S25] C：内存拷贝
来源：http://bxs.zdqjudy.top

memcpy(dst, src, n);
来源：http://xft.shzxlz.cn

[S26] C：内存清零
来源：http://wob.sweek.top


<!-- 参考信息 -->