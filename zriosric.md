代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pby.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://pbm.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tfm.tarul.cn

[Q57] 行号
来源：http://xun.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nje.zhixingplan.top

[Q58] 累计求和
来源：http://xcv.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fbm.hesvh.cn

[Q59] 分组内累计
来源：http://emo.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wme.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://zvi.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rpq.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lsu.yuanzhike.top

[Q61] 移动平均
来源：http://fti.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eqh.gotoacloud.top

[Q62] 分组占比
来源：http://ubh.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zbd.yfazqb.com

[Q63] 开启事务
来源：http://jdh.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jer.jyoumei.cn

[Q64] 提交事务
来源：http://oil.vehdjk.com

COMMIT;
来源：http://fds.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://ytl.9152youxi.cn

ROLLBACK;
来源：http://jpg.zhixingplan.top

[Q66] 行锁查询
来源：http://fru.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ofa.c1oappe.top

[Q67] 设置隔离级别
来源：http://emz.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hst.quarkkingdee.top

[Q68] 保存点
来源：http://rxd.yfazqb.com

SAVEPOINT sp1;
来源：http://blr.guannengcc.top

ROLLBACK TO sp1;
来源：http://hic.sxryk.cn

[Q69] 查看执行计划
来源：http://wrx.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ldh.epnwcf.com

[Q70] 更新统计信息
来源：http://yhp.jqgufenzy.top

ANALYZE TABLE users;
来源：http://mku.vqdsnc.cn

[Q71] 查看建表语句
来源：http://quy.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://puo.gzhubu.top

[Q72] 查看索引
来源：http://qmk.cucudq.cn

SHOW INDEX FROM users;
来源：http://uyy.zycfv.cn

[Q73] 查看表状态
来源：http://pss.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wtm.fktsv.cn

[Q74] 强制使用索引
来源：http://dix.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fbo.yvedp.cn

[Q75] 日期格式化
来源：http://lek.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cab.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zdv.jinqigfzy.top

[Q76] 按天统计
来源：http://mpk.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kxb.cheryme.top

[Q77] 时间加减
来源：http://obw.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uhz.tarul.cn

[Q78] 当前时间
来源：http://mwc.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ywv.guannengcc.top

[Q79] 字符串拼接
来源：http://ftl.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gfq.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://fjo.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oeo.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://rst.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qlz.tarul.cn

[Q82] 字符长度与字节长度
来源：http://uty.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bpb.fengsongda.top

[Q83] 大小写转换
来源：http://fkl.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://grx.sufxvd.cn

[Q84] 去除首尾空格
来源：http://mty.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://thz.sweek.top

[Q85] 数值取整
来源：http://vuh.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zpk.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://pbq.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ocm.guannengcc.top

[Q87] JSON 字段做条件
来源：http://cpo.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://joq.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://wtc.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://njz.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wja.cdnleiting.top

[Q89] 判断表是否存在
来源：http://gvu.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vsi.9152youxi.cn

[Q90] 生成序号列
来源：http://zzm.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fyi.aibaodan.cn

================================================================================
来源：http://ljc.ydjk.org.cn

R. Bash 专题
来源：http://doi.jlsjyb.cn

================================================================================
来源：http://wgv.0kj1m.cn

[R01] shebang 与严格模式
来源：http://nhi.guowangkeji.top

#!/usr/bin/env bash
来源：http://knw.haohaochexian.top

set -euo pipefail
来源：http://bzq.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://zcv.yangfankeji.com

name="Tom"; echo "$name"
来源：http://hek.quarkkingdee.top

[R03] 只读变量
来源：http://jrf.daxiang520.top

readonly PI=3.14
来源：http://rbx.xinyue.icu

[R04] 位置参数
来源：http://nsf.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zmk.dianchejie.cn

[R05] 参数默认值
来源：http://hxq.sufxvd.cn

name="${1:-default}"
来源：http://iib.sysykeji.top

[R06] 判断命令是否存在
来源：http://suc.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsg.yfazqb.com

[R07] if 判断文件
来源：http://vhs.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sbr.yj20258888.top

[R08] 数值比较
来源：http://cuw.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qfh.yueranfly.top

[R09] 字符串比较
来源：http://bcu.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://twi.yj202588.top

[R10] 正则匹配
来源：http://wqw.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cts.cucudq.cn

[R11] case 多分支
来源：http://mta.shanyushiyangkeji.top

case "$1" in
来源：http://dbd.kuanghao11.cn

start) echo "启动" ;;
来源：http://sjc.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://pgm.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://tyw.yvedp.cn

esac
来源：http://ccw.yangfankeji.com

[R12] for 遍历文件
来源：http://ebs.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://sjq.yuxming.cn

[R13] for 计数循环
来源：http://gly.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://nbh.xinyue.icu

[R14] C 风格 for
来源：http://rfo.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hcy.yvedp.cn

[R15] while 逐行读文件
来源：http://gon.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pfm.zhijiandao.cn

[R16] until 等待条件
来源：http://qsj.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xst.tanke756.top

[R17] 数组定义与取值
来源：http://pvz.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://qzf.birdmap.top

[R18] 遍历数组
来源：http://vne.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vqg.yvedp.cn

[R19] 数组长度
来源：http://afy.andypj.xyz

echo "${#arr[@]}"
来源：http://tbq.fehbvm.com

[R20] 关联数组（字典）
来源：http://bhy.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pkz.ydjk.org.cn

[R21] 字符串长度
来源：http://cxz.nanxuanxn.top

echo "${#s}"
来源：http://msc.316326.xyz

[R22] 截取子串
来源：http://tcl.gotoacloud.top

echo "${s:0:5}"
来源：http://kna.dashuyun.cn

[R23] 字符串替换
来源：http://zxt.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ugb.gotoacloud.top

[R24] 大小写转换
来源：http://azh.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://bza.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://cro.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://awe.dashuyun.cn

[R26] 命令替换
来源：http://tpx.yonumen.top

now=$(date +%F); echo "$now"
来源：http://iut.feifeiyinyue.top

[R27] 算术展开
来源：http://xcm.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://lpw.gzhubu.top

[R28] 浮点运算
来源：http://uzw.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://stx.vqdsnc.cn

[R29] 定义函数
来源：http://ctn.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wwh.gogol.net.cn

[R30] 函数返回状态码
来源：http://vrm.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://rig.yongpay.top

[R31] 局部变量
来源：http://rho.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://wku.gotoacloud.top

[R32] 参数个数校验
来源：http://urg.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bwh.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://wbc.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yjj.ydzc1.top

[R34] 退出时清理
来源：http://wcv.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://amb.bjfxy.top

[R35] 后台执行并等待
来源：http://wzo.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tce.tarul.cn

[R36] 并发执行多个任务
来源：http://kuy.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://unq.iojbl.cn

[R37] 把输出赋给变量
来源：http://aql.redwolf501.top

files=$(ls -1)
来源：http://irt.ppjwa.cn

[R38] 管道串联
来源：http://yak.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://bzh.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://asb.andypj.xyz

cmd > out.log 2>&1
来源：http://rjl.uphjek.com

[R40] 追加写日志
来源：http://oug.cucudq.cn

echo "log" >> out.log
来源：http://srg.fzhhl.top

[R41] 丢弃输出
来源：http://uob.yonumen.top

cmd >/dev/null 2>&1
来源：http://rok.quarkkingdee.top

[R42] 输入重定向
来源：http://jcu.tanke756.top

wc -l < a.txt
来源：http://lqe.hfpthk.cn

[R43] 按名字查找文件
来源：http://ksl.meibo888.top

find . -name "*.log" -type f
来源：http://fyx.vqdsnc.cn

[R44] 按修改时间查找
来源：http://vvp.xuanzx.com

find . -mtime -7 -type f
来源：http://ghp.kuanghao11.cn

[R45] 批量删除
来源：http://lpb.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://vzf.yueranfly.top

[R46] 递归替换文件内容
来源：http://fpx.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vgy.zhijiandao.cn

[R47] sed 单行替换
来源：http://kiu.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://swp.yj20258888.top

[R48] awk 取指定列
来源：http://odm.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://fhm.hysaishi.cn

[R49] awk 带条件
来源：http://diy.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xqu.fktsv.cn

[R50] awk 求和
来源：http://jjy.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vpy.gaohongyu789.top

[R51] 排序去重取前几
来源：http://btq.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ccl.pengpengdd.cyou

[R52] 统计行数
来源：http://jfu.316326.xyz

wc -l a.txt
来源：http://rdq.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://uoh.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zcb.zycfv.cn

[R54] 比较两个文件
来源：http://vte.jqgufenzy.top

diff a.txt b.txt
来源：http://nph.aizwys.cn

[R55] 压缩与解压
来源：http://zsi.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vwa.smart0.xyz

[R56] 远程拷贝
来源：http://wrk.chenlongwang.top

scp file user@host:/path/
来源：http://xzt.birdmap.top

[R57] 远程执行命令
来源：http://gqx.zdqjudy.top

ssh user@host 'uptime'
来源：http://wxa.zhengqikj.top

[R58] 下载文件
来源：http://tvb.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://amr.pycfn.com

[R59] 发 POST JSON
来源：http://rnh.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ulw.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://eme.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://edl.hammf.cn

[R61] 磁盘占用
来源：http://atd.redwolf501.top

df -h;  du -sh *
来源：http://qcv.pycfn.com

[R62] 找最占空间的文件
来源：http://hrl.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://wsu.kuanghao11.cn

[R63] 内存与进程
来源：http://urw.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://bbl.yfazqb.com

[R64] 结束进程
来源：http://mnw.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://zgi.hammf.cn

[R65] 查看端口占用
来源：http://ojh.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xjb.jiagoushi.top

[R66] 定时任务
来源：http://tox.chenzaomai.com

crontab -e;  crontab -l
来源：http://qfo.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://zjs.yanxiufei.cn

openssl rand -hex 16
来源：http://dha.yvedp.cn

[R68] 计算文件校验值
来源：http://rys.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://gui.iojbl.cn

[R69] 生成随机密码
来源：http://wjj.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://avs.zhoulong.xyz

[R70] 时间戳与互转
来源：http://gxs.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://mcz.yuanzhike.top

[R71] 日期格式化
来源：http://ldm.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lyw.hfpthk.cn

[R72] 等待端口就绪
来源：http://urt.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://brv.yueranfly.top

[R73] 分割大日志
来源：http://vln.zhongyouzk.top

split -l 1000 big.log part_
来源：http://qpv.fengsongda.top

[R74] 批量重命名
来源：http://pdp.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://omc.ctjpmb.com

[R75] 导出环境变量
来源：http://vbz.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://ahp.c1oappe.top

[R76] 使用临时文件
来源：http://eyx.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bny.chenlongwang.top

[R77] 读取用户输入
来源：http://mtc.yj202588.top

read -rp "请输入: " ans
来源：http://hag.fengsongda.top

[R78] 交互式菜单
来源：http://whn.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://chy.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://bse.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gom.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://ule.yanxiufei.cn

time ./run.sh
来源：http://hta.haohaochexian.top

================================================================================
来源：http://fdg.tanke756.top

S. C / C++ 专题
来源：http://rvq.yj202588.top

================================================================================
来源：http://ezx.zdbjq.cn

[S01] C：Hello World
来源：http://kra.xziqi.cn

#include <stdio.h>
来源：http://aei.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hiq.yonumen.top

[S02] C：变量与格式化输出
来源：http://sfy.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://cyy.nwbrower.top

[S03] C：读入整数
来源：http://nav.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://uki.shzxlz.cn

[S04] C：字符串复制
来源：http://iod.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://hdf.hnxiangtu.top

[S05] C：字符串长度
来源：http://wml.dianchejie.cn

strlen(s)
来源：http://yqm.ppjwa.cn

[S06] C：字符串比较
来源：http://lua.sxryk.cn

strcmp(a, b) == 0
来源：http://gom.hfpthk.cn

[S07] C：数组遍历求和
来源：http://zuh.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://giw.316326.xyz

[S08] C：动态内存分配与释放
来源：http://sta.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mvc.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://xtn.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cyr.0kj1m.cn

[S10] C：指针与解引用
来源：http://hrz.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://ovd.hysaishi.cn

[S11] C：逐行读文件
来源：http://thz.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://caz.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://pom.zhengqikj.top

fclose(f);
来源：http://tgs.xinyue.icu

[S12] C：写文件
来源：http://kql.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqr.yuxming.cn

[S13] C：宏定义
来源：http://zqq.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yjm.yj202588.top

[S14] C：枚举
来源：http://xul.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://ewr.yfazqb.com

[S15] C：类型转换
来源：http://jtj.fanxiaobao.xyz

(double) a / b
来源：http://mld.zhijiandao.cn

[S16] C：位操作置位
来源：http://mrm.chenzaomai.com

x |= (1 << 3);
来源：http://etp.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://sxv.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aqz.gogol.net.cn

[S18] C：命令行参数
来源：http://eao.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://yaj.fzhhl.top

[S19] C：快速排序
来源：http://khb.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://kdu.tianlin.xyz

[S20] C：二分查找
来源：http://mxp.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wkr.wangdashe.top

[S21] C：字符类别判断
来源：http://rtb.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://osj.tianlin.xyz

[S22] C：字符串转数字
来源：http://gwc.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://vdd.xziqi.cn

[S23] C：随机数
来源：http://xke.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dlm.dianchejie.cn

[S24] C：获取本地时间
来源：http://jkp.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xxv.kuanghao11.cn

[S25] C：内存拷贝
来源：http://tvz.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://vng.zycfv.cn

[S26] C：内存清零
来源：http://hcw.iojbl.cn


<!-- 参考信息 -->