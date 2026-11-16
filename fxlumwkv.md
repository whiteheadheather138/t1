代发 wailian999

[Q65] 回滚事务
来源：http://qrw.sxryk.cn

ROLLBACK;
来源：http://pfg.316326.xyz

[Q66] 行锁查询
来源：http://tms.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yhz.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://jjp.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hia.jinghuilouyu.cn

[Q68] 保存点
来源：http://amc.bbcook.cn

SAVEPOINT sp1;
来源：http://mhm.wangdashe.top

ROLLBACK TO sp1;
来源：http://svs.nanxinkj.top

[Q69] 查看执行计划
来源：http://hgk.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eao.meibo888.top

[Q70] 更新统计信息
来源：http://vea.zhoulong.xyz

ANALYZE TABLE users;
来源：http://dlz.0kj1m.cn

[Q71] 查看建表语句
来源：http://sol.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qtk.yj202588.top

[Q72] 查看索引
来源：http://vxn.yj20258888.top

SHOW INDEX FROM users;
来源：http://xem.zdbjq.cn

[Q73] 查看表状态
来源：http://rpy.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uvl.yj202588.top

[Q74] 强制使用索引
来源：http://wwb.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nub.hywenlv.cn

[Q75] 日期格式化
来源：http://voe.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ueb.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jjl.jqgfzy.top

[Q76] 按天统计
来源：http://ikm.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nnf.ivvv.top

[Q77] 时间加减
来源：http://rcu.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tga.xuetiantiany.cn

[Q78] 当前时间
来源：http://dpm.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oke.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://caj.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vgr.guowangkeji.top

[Q80] 字符串截取
来源：http://oho.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bqb.xinyue.icu

[Q81] 字符串替换
来源：http://aug.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hcs.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://cfs.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dvv.chenzaomai.com

[Q83] 大小写转换
来源：http://xqk.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://orh.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://tcf.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://kuu.shuidangran.top

[Q85] 数值取整
来源：http://oph.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://crz.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://tbg.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bda.ydzc1.top

[Q87] JSON 字段做条件
来源：http://mpr.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yqo.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://nnj.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rsf.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ade.smart0.xyz

[Q89] 判断表是否存在
来源：http://ftf.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rhf.meibo888.top

[Q90] 生成序号列
来源：http://wav.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oab.svipenyu.cn

================================================================================
来源：http://qvd.yuanzhike.top

R. Bash 专题
来源：http://tle.yangfankeji.com

================================================================================
来源：http://tmt.ybcxt.top

[R01] shebang 与严格模式
来源：http://xlq.sjlbkw.cn

#!/usr/bin/env bash
来源：http://ona.wangshuangyany.cn

set -euo pipefail
来源：http://imr.yvedp.cn

[R02] 变量赋值与使用
来源：http://mbo.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://cew.tarul.cn

[R03] 只读变量
来源：http://aef.tian-w.cn

readonly PI=3.14
来源：http://eqp.zhengqikj.top

[R04] 位置参数
来源：http://wjb.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qfy.jqgfzy.top

[R05] 参数默认值
来源：http://all.cqqwz.cn

name="${1:-default}"
来源：http://lia.birdmap.top

[R06] 判断命令是否存在
来源：http://evd.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pkk.ivvv.top

[R07] if 判断文件
来源：http://avq.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ppp.hywenlv.cn

[R08] 数值比较
来源：http://rli.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kzp.bjfxy.top

[R09] 字符串比较
来源：http://hrz.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cso.yueranfly.top

[R10] 正则匹配
来源：http://djo.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pnr.gaohongyu789.top

[R11] case 多分支
来源：http://buf.jinghuilouyu.cn

case "$1" in
来源：http://gfz.mhx1999.top

start) echo "启动" ;;
来源：http://sfq.tian-w.cn

stop)  echo "停止" ;;
来源：http://wka.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://oeq.ydzc1.top

esac
来源：http://fby.cheryme.top

[R12] for 遍历文件
来源：http://idh.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://oly.tianlin.xyz

[R13] for 计数循环
来源：http://rsv.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://akd.wangdashe.top

[R14] C 风格 for
来源：http://hwe.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fbt.sxryk.cn

[R15] while 逐行读文件
来源：http://emb.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ndc.zhiwuduotai.top

[R16] until 等待条件
来源：http://zyz.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://urb.cucudq.cn

[R17] 数组定义与取值
来源：http://mbe.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mza.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://tiy.andypj.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://reu.guannengcc.top

[R19] 数组长度
来源：http://ejt.316326.xyz

echo "${#arr[@]}"
来源：http://shc.zdbjq.cn

[R20] 关联数组（字典）
来源：http://dxr.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qll.vehdjk.com

[R21] 字符串长度
来源：http://nhs.tarul.cn

echo "${#s}"
来源：http://fcl.yj20258888.top

[R22] 截取子串
来源：http://npi.chenlongwang.top

echo "${s:0:5}"
来源：http://xul.xinyue.icu

[R23] 字符串替换
来源：http://keu.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dta.c1oappe.top

[R24] 大小写转换
来源：http://bwd.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://uou.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://caw.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://byl.cheryme.top

[R26] 命令替换
来源：http://elf.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://kmj.zycfv.cn

[R27] 算术展开
来源：http://yvp.yvedp.cn

echo $((1 + 2 * 3))
来源：http://cka.zhengqikj.top

[R28] 浮点运算
来源：http://sxa.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://mhp.andypj.xyz

[R29] 定义函数
来源：http://mot.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wys.tanke756.top

[R30] 函数返回状态码
来源：http://fqo.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://pss.tanke756.top

[R31] 局部变量
来源：http://sxm.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://cog.bbcook.cn

[R32] 参数个数校验
来源：http://loj.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xmq.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://hir.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ldq.tian-w.cn

[R34] 退出时清理
来源：http://mdm.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tzq.xuanzx.com

[R35] 后台执行并等待
来源：http://qyy.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zlg.sufxvd.cn

[R36] 并发执行多个任务
来源：http://cwb.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rue.meibo888.top

[R37] 把输出赋给变量
来源：http://cdc.gzhubu.top

files=$(ls -1)
来源：http://cxw.wangshuangyany.cn

[R38] 管道串联
来源：http://fwu.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://ihu.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://amk.iojbl.cn

cmd > out.log 2>&1
来源：http://ltz.pycfn.com

[R40] 追加写日志
来源：http://jtr.redwolf501.top

echo "log" >> out.log
来源：http://yot.hnqzz.top

[R41] 丢弃输出
来源：http://odx.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://vkn.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://moz.zdqjudy.top

wc -l < a.txt
来源：http://slu.cdnleiting.top

[R43] 按名字查找文件
来源：http://afm.snrcjt.cn

find . -name "*.log" -type f
来源：http://ydr.yvedp.cn

[R44] 按修改时间查找
来源：http://sfe.kuanghao11.cn

find . -mtime -7 -type f
来源：http://uxc.jinqigfzy.top

[R45] 批量删除
来源：http://gkr.tian-w.cn

find . -name "*.tmp" -delete
来源：http://sus.bbcook.cn

[R46] 递归替换文件内容
来源：http://ati.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vio.vehdjk.com

[R47] sed 单行替换
来源：http://dcn.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://lwb.hywenlv.cn

[R48] awk 取指定列
来源：http://icw.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://trf.sweek.top

[R49] awk 带条件
来源：http://zvz.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cmk.9152youxi.cn

[R50] awk 求和
来源：http://uld.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://ihz.jyoumei.cn

[R51] 排序去重取前几
来源：http://wpg.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oia.hywenlv.cn

[R52] 统计行数
来源：http://xmv.pengpengdd.cyou

wc -l a.txt
来源：http://kuw.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://xcx.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yow.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://ldh.bbcook.cn

diff a.txt b.txt
来源：http://nif.svipenyu.cn

[R55] 压缩与解压
来源：http://lyx.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kpe.zhongyouzk.top

[R56] 远程拷贝
来源：http://mgc.daxiang520.top

scp file user@host:/path/
来源：http://zrw.hammf.cn

[R57] 远程执行命令
来源：http://tjo.jiagoushi.top

ssh user@host 'uptime'
来源：http://fzy.zhoulong.xyz

[R58] 下载文件
来源：http://hto.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vdj.fengsongda.top

[R59] 发 POST JSON
来源：http://zhp.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jqd.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://ixc.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nld.shangyingyoupin.top

[R61] 磁盘占用
来源：http://fqa.cqqwz.cn

df -h;  du -sh *
来源：http://pvc.ydzc1.top

[R62] 找最占空间的文件
来源：http://qxc.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://gla.pycfn.com

[R63] 内存与进程
来源：http://bgs.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://ouc.cqqwz.cn

[R64] 结束进程
来源：http://ygo.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://xll.birdmap.top

[R65] 查看端口占用
来源：http://sbb.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wwx.ydzc1.top

[R66] 定时任务
来源：http://wkr.cdnleiting.top

crontab -e;  crontab -l
来源：http://hne.meibo888.top

[R67] 生成随机十六进制串
来源：http://jvw.pengpengdd.cyou

openssl rand -hex 16
来源：http://okw.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://hue.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://zfl.svipenyu.cn

[R69] 生成随机密码
来源：http://fgh.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://hch.cucudq.cn

[R70] 时间戳与互转
来源：http://hkv.aizwys.cn

date +%s;  date -d @1700000000
来源：http://ulp.gzhubu.top

[R71] 日期格式化
来源：http://ofp.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jwa.mhx1999.top

[R72] 等待端口就绪
来源：http://wiq.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vwb.yj20258.top

[R73] 分割大日志
来源：http://tgq.zycfv.cn

split -l 1000 big.log part_
来源：http://fyu.andypj.xyz

[R74] 批量重命名
来源：http://vxd.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eod.gaohongyu789.top

[R75] 导出环境变量
来源：http://wan.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://ufr.smart0.xyz

[R76] 使用临时文件
来源：http://opp.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fyj.gogol.net.cn

[R77] 读取用户输入
来源：http://ocl.yanxiufei.cn

read -rp "请输入: " ans
来源：http://bow.gogol.net.cn

[R78] 交互式菜单
来源：http://vjq.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gsz.jinqigufen.top

[R79] 解析命令行选项
来源：http://jbn.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://roy.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://iop.guannengcc.top

time ./run.sh
来源：http://txj.yvedp.cn

================================================================================
来源：http://feu.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://mwe.yongpay.top

================================================================================
来源：http://gga.daxiang520.top

[S01] C：Hello World
来源：http://pnh.chenjidiqi.icu

#include <stdio.h>
来源：http://vjx.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ene.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://zol.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://ijc.yangfankeji.com

[S03] C：读入整数
来源：http://xmy.jiagoushi.top

int x; scanf("%d", &x);
来源：http://qae.kuanghao11.cn

[S04] C：字符串复制
来源：http://tum.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hcw.yanxiufei.cn

[S05] C：字符串长度
来源：http://eav.jinghuilouyu.cn

strlen(s)
来源：http://pgp.aizwys.cn

[S06] C：字符串比较
来源：http://ldo.fehbvm.com

strcmp(a, b) == 0
来源：http://uvf.ydzc1.top

[S07] C：数组遍历求和
来源：http://zys.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jdc.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://rcx.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kpa.uphjek.com

[S09] C：结构体定义与初始化
来源：http://zth.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://prd.zdqjudy.top

[S10] C：指针与解引用
来源：http://spi.bbcook.cn

int *p = &a;  *p = 5;
来源：http://eyb.yfazqb.com

[S11] C：逐行读文件
来源：http://afj.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://nrf.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://bjf.hysaishi.cn

fclose(f);
来源：http://mbp.hnqzz.top

[S12] C：写文件
来源：http://saf.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://odt.yongpay.top

[S13] C：宏定义
来源：http://nsv.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nqc.zycfv.cn

[S14] C：枚举
来源：http://wvs.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://mnk.xingfuxueyuan.xyz

[S15] C：类型转换
来源：http://bqj.xuetiantiany.cn

(double) a / b
来源：http://xyq.xuetiantiany.cn

[S16] C：位操作置位
来源：http://vvu.hcnkem.com

x |= (1 << 3);
来源：http://fvg.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://bzr.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nrz.svipenyu.cn

[S18] C：命令行参数
来源：http://vyl.jinghuilouyu.cn

int main(int argc, char **argv)
来源：http://jrk.ppjwa.cn

[S19] C：快速排序
来源：http://sri.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://tlr.hysaishi.cn

[S20] C：二分查找
来源：http://qjf.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://smp.tianlin.xyz

[S21] C：字符类别判断
来源：http://gba.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wum.quarkkingdee.top

[S22] C：字符串转数字
来源：http://tbd.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nqf.zycfv.cn

[S23] C：随机数
来源：http://wud.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rwu.havefunace.top

[S24] C：获取本地时间
来源：http://knd.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cgj.jlsjyb.cn

[S25] C：内存拷贝
来源：http://upn.jinqigfzy.top

memcpy(dst, src, n);
来源：http://elt.sxryk.cn

[S26] C：内存清零
来源：http://szp.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://ebr.hammf.cn

[S27] C：定义常量
来源：http://xuj.yfazqb.com

const double PI = 3.14159;
来源：http://meq.jyoumei.cn

[S28] C：静态变量
来源：http://xiw.gogol.net.cn

static int counter = 0;
来源：http://qdh.cashguo.top

[S29] C：变参函数
来源：http://kdr.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://spa.haohaochexian.top

[S30] C：头文件保护
来源：http://xoa.cucudq.cn

#ifndef X_H
来源：http://nei.tarul.cn

#define X_H
来源：http://xly.xylfe.cn

#endif
来源：http://vfu.hammf.cn

[S31] C++：Hello World
来源：http://gpf.gaohongyu789.top

#include <iostream>
来源：http://kcc.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://puv.jinqigfzy.top

[S32] C++：字符串
来源：http://son.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://weq.nanxinkj.top

[S33] C++：vector 增删
来源：http://irg.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://plm.guannengcc.top

[S34] C++：遍历 vector
来源：http://fkw.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://okx.jyoumei.cn


<!-- 参考信息 -->