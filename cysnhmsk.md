代发 wailian999

[Q67] 设置隔离级别
来源：http://cqh.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://icr.zycfv.cn

[Q68] 保存点
来源：http://dka.shuidangran.top

SAVEPOINT sp1;
来源：http://xyo.redwolf501.top

ROLLBACK TO sp1;
来源：http://xeq.fktsv.cn

[Q69] 查看执行计划
来源：http://cak.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qqe.cucudq.cn

[Q70] 更新统计信息
来源：http://uji.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://xqw.gogol.net.cn

[Q71] 查看建表语句
来源：http://oam.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ymq.sxryk.cn

[Q72] 查看索引
来源：http://giw.guowangkeji.top

SHOW INDEX FROM users;
来源：http://kba.xylfe.cn

[Q73] 查看表状态
来源：http://hnp.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kto.guannengcc.top

[Q74] 强制使用索引
来源：http://aer.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ogs.zhoulong.xyz

[Q75] 日期格式化
来源：http://kky.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wzy.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jpk.guowangkeji.top

[Q76] 按天统计
来源：http://bmg.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tuq.hongshengwenyu.top

[Q77] 时间加减
来源：http://emw.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kqp.kuanghao11.cn

[Q78] 当前时间
来源：http://wlm.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qjh.c1oappe.top

[Q79] 字符串拼接
来源：http://wtx.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dlg.daria6918.cn

[Q80] 字符串截取
来源：http://utq.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hxb.ctjpmb.com

[Q81] 字符串替换
来源：http://zpl.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bvd.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://wer.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vvk.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://cpd.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ejp.yonumen.top

[Q84] 去除首尾空格
来源：http://nzn.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://nwu.bbcook.cn

[Q85] 数值取整
来源：http://gsf.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://djc.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://bjy.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cnn.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://kyq.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mdg.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://hmn.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ecn.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xng.ctjpmb.com

[Q89] 判断表是否存在
来源：http://kuo.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ufs.gzhubu.top

[Q90] 生成序号列
来源：http://ihe.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yum.dianchejie.cn

================================================================================
来源：http://vnt.0kj1m.cn

R. Bash 专题
来源：http://zix.hfpthk.cn

================================================================================
来源：http://col.sweek.top

[R01] shebang 与严格模式
来源：http://qwe.jyoumei.cn

#!/usr/bin/env bash
来源：http://hpz.xuanzx.com

set -euo pipefail
来源：http://muc.daxiang520.top

[R02] 变量赋值与使用
来源：http://knz.52xcode.cn

name="Tom"; echo "$name"
来源：http://vxw.tanke756.top

[R03] 只读变量
来源：http://zic.hywenlv.cn

readonly PI=3.14
来源：http://twa.hywenlv.cn

[R04] 位置参数
来源：http://hfg.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xpv.xuetiantiany.cn

[R05] 参数默认值
来源：http://pvd.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://fdz.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://vzq.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ydr.yonumen.top

[R07] if 判断文件
来源：http://kur.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://muy.fehbvm.com

[R08] 数值比较
来源：http://hsp.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://alz.svipenyu.cn

[R09] 字符串比较
来源：http://fbl.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hpm.yonumen.top

[R10] 正则匹配
来源：http://wyv.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dpi.quarkkingdee.top

[R11] case 多分支
来源：http://blh.xziqi.cn

case "$1" in
来源：http://ykf.cucudq.cn

start) echo "启动" ;;
来源：http://lbn.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://cdx.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://zqp.shangyingyoupin.top

esac
来源：http://kdd.fktsv.cn

[R12] for 遍历文件
来源：http://gmc.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://phx.svipenyu.cn

[R13] for 计数循环
来源：http://mnr.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://eaf.nanxinkj.top

[R14] C 风格 for
来源：http://fmk.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hje.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://epm.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://htq.jqgfzy.top

[R16] until 等待条件
来源：http://uba.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gpd.ctjpmb.com

[R17] 数组定义与取值
来源：http://ldp.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ejh.xziqi.cn

[R18] 遍历数组
来源：http://zzg.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fsm.tanke756.top

[R19] 数组长度
来源：http://yfy.andypj.xyz

echo "${#arr[@]}"
来源：http://sfq.zdqjudy.top

[R20] 关联数组（字典）
来源：http://jgt.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://euo.jianghu66.top

[R21] 字符串长度
来源：http://lla.yvedp.cn

echo "${#s}"
来源：http://rjy.nanxuanxn.top

[R22] 截取子串
来源：http://tss.mhx1999.top

echo "${s:0:5}"
来源：http://ked.0kj1m.cn

[R23] 字符串替换
来源：http://pta.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dyg.cheryme.top

[R24] 大小写转换
来源：http://yvo.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://tfv.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://hgf.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xju.shangyingyoupin.top

[R26] 命令替换
来源：http://eeu.cashguo.top

now=$(date +%F); echo "$now"
来源：http://plx.yueranfly.top

[R27] 算术展开
来源：http://sqv.yongpay.top

echo $((1 + 2 * 3))
来源：http://gyu.shanyushiyangtech.top

[R28] 浮点运算
来源：http://fqt.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://fgq.yueranfly.top

[R29] 定义函数
来源：http://aiw.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hlj.yj20258888.top

[R30] 函数返回状态码
来源：http://iup.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://gyh.sxryk.cn

[R31] 局部变量
来源：http://scm.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://ktn.0kj1m.cn

[R32] 参数个数校验
来源：http://igy.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hrp.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://iir.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gid.wangshuangyany.cn

[R34] 退出时清理
来源：http://khr.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kqg.snrcjt.cn

[R35] 后台执行并等待
来源：http://tel.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://egv.cashguo.top

[R36] 并发执行多个任务
来源：http://iec.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bho.yuxming.cn

[R37] 把输出赋给变量
来源：http://vih.jinqigufen.top

files=$(ls -1)
来源：http://bhk.ywan-chungtsiang.top

[R38] 管道串联
来源：http://mbt.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://xou.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://znd.dianchejie.cn

cmd > out.log 2>&1
来源：http://xmo.zhongyouzk.top

[R40] 追加写日志
来源：http://hbd.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://une.sjlbkw.cn

[R41] 丢弃输出
来源：http://iei.52xcode.cn

cmd >/dev/null 2>&1
来源：http://fcv.yongpay.top

[R42] 输入重定向
来源：http://eyi.hnqzz.top

wc -l < a.txt
来源：http://bzi.xziqi.cn

[R43] 按名字查找文件
来源：http://fxe.zhengqikj.top

find . -name "*.log" -type f
来源：http://wcz.epnwcf.com

[R44] 按修改时间查找
来源：http://zla.yanxiufei.cn

find . -mtime -7 -type f
来源：http://oqf.yvedp.cn

[R45] 批量删除
来源：http://btg.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://ycv.fktsv.cn

[R46] 递归替换文件内容
来源：http://dlg.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gus.zdqjudy.top

[R47] sed 单行替换
来源：http://erj.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://qcr.bbcook.cn

[R48] awk 取指定列
来源：http://rgi.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://lvc.jinqigfzy.top

[R49] awk 带条件
来源：http://ypc.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mdv.fktsv.cn

[R50] awk 求和
来源：http://ikw.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uzv.shzxlz.cn

[R51] 排序去重取前几
来源：http://nwc.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gyi.epnwcf.com

[R52] 统计行数
来源：http://wtc.jinqigufen.top

wc -l a.txt
来源：http://hgt.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://von.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sdj.jinqigfzy.top

[R54] 比较两个文件
来源：http://xoj.pycfn.com

diff a.txt b.txt
来源：http://xme.fehbvm.com

[R55] 压缩与解压
来源：http://nxw.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ywv.svipenyu.cn

[R56] 远程拷贝
来源：http://sgi.yj20258.top

scp file user@host:/path/
来源：http://wlo.cashguo.top

[R57] 远程执行命令
来源：http://gyc.xziqi.cn

ssh user@host 'uptime'
来源：http://rfw.fengsongda.top

[R58] 下载文件
来源：http://svt.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mfh.tian-w.cn

[R59] 发 POST JSON
来源：http://nfr.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qlv.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://qzr.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pet.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://qlp.jianghu66.top

df -h;  du -sh *
来源：http://iyf.bbcook.cn

[R62] 找最占空间的文件
来源：http://cct.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://ogs.sysykeji.top

[R63] 内存与进程
来源：http://pvn.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://eem.shzxlz.cn

[R64] 结束进程
来源：http://raw.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://ztu.chenlongwang.top

[R65] 查看端口占用
来源：http://sds.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dsj.ppjwa.cn

[R66] 定时任务
来源：http://rxd.zhengqikj.top

crontab -e;  crontab -l
来源：http://zca.52xcode.cn

[R67] 生成随机十六进制串
来源：http://ocy.zhengqikj.top

openssl rand -hex 16
来源：http://wzo.sufxvd.cn

[R68] 计算文件校验值
来源：http://hdh.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pej.jiagoushi.top

[R69] 生成随机密码
来源：http://udl.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://zyk.snrcjt.cn

[R70] 时间戳与互转
来源：http://vdz.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://riv.shanyushiyangtech.top

[R71] 日期格式化
来源：http://wxi.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://bcv.hysaishi.cn

[R72] 等待端口就绪
来源：http://box.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bhf.ctjpmb.com

[R73] 分割大日志
来源：http://zlx.chenlongwang.top

split -l 1000 big.log part_
来源：http://gxr.jqgufenzy.top

[R74] 批量重命名
来源：http://pxh.tarul.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vnq.iojbl.cn

[R75] 导出环境变量
来源：http://sfy.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://hll.ctjpmb.com

[R76] 使用临时文件
来源：http://fxo.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rch.birdmap.top

[R77] 读取用户输入
来源：http://rim.hcnkem.com

read -rp "请输入: " ans
来源：http://rja.snrcjt.cn

[R78] 交互式菜单
来源：http://gtf.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xxz.nwbrower.top

[R79] 解析命令行选项
来源：http://bxq.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tmj.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://twk.yj20258.top

time ./run.sh
来源：http://qdc.yueranfly.top

================================================================================
来源：http://cki.hnxiangtu.top

S. C / C++ 专题
来源：http://umw.vqdsnc.cn

================================================================================
来源：http://ccx.guowangkeji.top

[S01] C：Hello World
来源：http://qam.ppjwa.cn

#include <stdio.h>
来源：http://bjn.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://svo.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://mja.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://kjz.wangdashe.top

[S03] C：读入整数
来源：http://pso.sysykeji.top

int x; scanf("%d", &x);
来源：http://cbo.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://ygc.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://pka.gogol.net.cn

[S05] C：字符串长度
来源：http://mpr.yj20258.top

strlen(s)
来源：http://uyx.zhengqikj.top

[S06] C：字符串比较
来源：http://gfn.nwbrower.top

strcmp(a, b) == 0
来源：http://ill.tianlin.xyz

[S07] C：数组遍历求和
来源：http://hjf.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://icb.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://idd.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tep.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://qak.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eeq.sxryk.cn

[S10] C：指针与解引用
来源：http://hkr.cucudq.cn

int *p = &a;  *p = 5;
来源：http://cwk.zhixingplan.top

[S11] C：逐行读文件
来源：http://jkl.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://skw.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kfp.feifeiyinyue.top

fclose(f);
来源：http://epo.ctjpmb.com

[S12] C：写文件
来源：http://iwh.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jue.yanxiufei.cn

[S13] C：宏定义
来源：http://wvf.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://epx.shanyushiyangtech.top

[S14] C：枚举
来源：http://mwa.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://ddb.fehbvm.com

[S15] C：类型转换
来源：http://xdx.zhongyouzk.top

(double) a / b
来源：http://pbd.yanxiufei.cn

[S16] C：位操作置位
来源：http://fgu.xuetiantiany.cn

x |= (1 << 3);
来源：http://eob.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://xch.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lbn.chenlongwang.top

[S18] C：命令行参数
来源：http://rog.uphjek.com

int main(int argc, char **argv)
来源：http://ntv.shuidangran.top

[S19] C：快速排序
来源：http://qiy.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://hdk.zhoulong.xyz

[S20] C：二分查找
来源：http://gzj.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jnr.jiagoushi.top

[S21] C：字符类别判断
来源：http://doj.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kgh.hesvh.cn

[S22] C：字符串转数字
来源：http://uec.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://cwp.tianlin.xyz

[S23] C：随机数
来源：http://crb.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://agu.jqgufenzy.top

[S24] C：获取本地时间
来源：http://vky.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kce.nanxuanxn.top

[S25] C：内存拷贝
来源：http://pdy.9152youxi.cn

memcpy(dst, src, n);
来源：http://iuq.vehdjk.com

[S26] C：内存清零
来源：http://pqt.tarul.cn

memset(a, 0, sizeof a);
来源：http://yys.ppjwa.cn

[S27] C：定义常量
来源：http://tnn.0kj1m.cn

const double PI = 3.14159;
来源：http://cea.fktsv.cn

[S28] C：静态变量
来源：http://ctd.9152youxi.cn

static int counter = 0;
来源：http://euw.quarkkingdee.top

[S29] C：变参函数
来源：http://asz.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zdv.yanxiufei.cn

[S30] C：头文件保护
来源：http://ouv.zycfv.cn

#ifndef X_H
来源：http://tvq.gaohongyu789.top

#define X_H
来源：http://jms.cashguo.top

#endif
来源：http://eob.nanxuanxn.top

[S31] C++：Hello World
来源：http://woy.aibaodan.cn

#include <iostream>
来源：http://iga.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://eni.andypj.xyz

[S32] C++：字符串
来源：http://wlv.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://cdd.yanxiufei.cn

[S33] C++：vector 增删
来源：http://tsm.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xll.cqqwz.cn

[S34] C++：遍历 vector
来源：http://ytu.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://mpd.sysykeji.top

[S35] C++：map
来源：http://aeq.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zfd.jianghu66.top

[S36] C++：unordered_map
来源：http://xvs.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gov.316326.xyz


<!-- 参考信息 -->