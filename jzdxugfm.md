代发 wailian999

ROLLBACK TO sp1;
来源：http://lut.tarul.cn

[Q69] 查看执行计划
来源：http://got.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nuc.sweek.top

[Q70] 更新统计信息
来源：http://xjv.yj20258888.top

ANALYZE TABLE users;
来源：http://olb.redwolf501.top

[Q71] 查看建表语句
来源：http://gct.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oir.wangshuangyany.cn

[Q72] 查看索引
来源：http://wfa.sxryk.cn

SHOW INDEX FROM users;
来源：http://nvx.mhx1999.top

[Q73] 查看表状态
来源：http://piz.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pvl.dashuyun.cn

[Q74] 强制使用索引
来源：http://vxj.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://owx.cheryme.top

[Q75] 日期格式化
来源：http://vyk.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lgk.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sly.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://lee.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uzg.ydzc1.top

[Q77] 时间加减
来源：http://quo.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ujy.yvedp.cn

[Q78] 当前时间
来源：http://vli.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bph.aibaodan.cn

[Q79] 字符串拼接
来源：http://ixj.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://btx.jianghu66.top

[Q80] 字符串截取
来源：http://ezw.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zmo.yongpay.top

[Q81] 字符串替换
来源：http://lim.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nhl.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://uau.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eth.hammf.cn

[Q83] 大小写转换
来源：http://jjp.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lkc.tarul.cn

[Q84] 去除首尾空格
来源：http://qfk.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://fzg.52xcode.cn

[Q85] 数值取整
来源：http://lli.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jan.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://hxa.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gal.jianghu66.top

[Q87] JSON 字段做条件
来源：http://wfu.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zcv.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://vdw.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lpx.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ftm.sweek.top

[Q89] 判断表是否存在
来源：http://tvq.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zkg.chenlongwang.top

[Q90] 生成序号列
来源：http://qsz.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lac.shanyushiyangkeji.top

================================================================================
来源：http://pim.ivvv.top

R. Bash 专题
来源：http://obp.fktsv.cn

================================================================================
来源：http://ijn.ybcxt.top

[R01] shebang 与严格模式
来源：http://nwr.fzhhl.top

#!/usr/bin/env bash
来源：http://wcf.aibaodan.cn

set -euo pipefail
来源：http://kui.wangdashe.top

[R02] 变量赋值与使用
来源：http://kty.birdmap.top

name="Tom"; echo "$name"
来源：http://tex.meibo888.top

[R03] 只读变量
来源：http://qqk.hesvh.cn

readonly PI=3.14
来源：http://hoy.xinyue.icu

[R04] 位置参数
来源：http://fng.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qzh.shanyushiyangtech.top

[R05] 参数默认值
来源：http://gxh.xylfe.cn

name="${1:-default}"
来源：http://ekq.wangdashe.top

[R06] 判断命令是否存在
来源：http://ico.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uiw.kuanghao11.cn

[R07] if 判断文件
来源：http://awk.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tgj.yonumen.top

[R08] 数值比较
来源：http://ntb.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://cyp.hesvh.cn

[R09] 字符串比较
来源：http://ixf.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ldm.haohaochexian.top

[R10] 正则匹配
来源：http://qzn.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uac.feifeiyinyue.top

[R11] case 多分支
来源：http://jiv.xinyue.icu

case "$1" in
来源：http://rtr.9152youxi.cn

start) echo "启动" ;;
来源：http://akz.dianchejie.cn

stop)  echo "停止" ;;
来源：http://pey.pycfn.com

*)     echo "未知命令" ;;
来源：http://dpy.hongshengwenyu.top

esac
来源：http://yyy.cucudq.cn

[R12] for 遍历文件
来源：http://lrx.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://toh.sufxvd.cn

[R13] for 计数循环
来源：http://scr.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://hpm.cqqwz.cn

[R14] C 风格 for
来源：http://jkd.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://syn.jinqigfzy.top

[R15] while 逐行读文件
来源：http://ozl.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hau.vehdjk.com

[R16] until 等待条件
来源：http://cgl.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fqn.ivvv.top

[R17] 数组定义与取值
来源：http://xdu.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://ccw.dashuyun.cn

[R18] 遍历数组
来源：http://fwz.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oqr.ydzc1.top

[R19] 数组长度
来源：http://csg.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://wtg.iojbl.cn

[R20] 关联数组（字典）
来源：http://zyj.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fap.yfazqb.com

[R21] 字符串长度
来源：http://guo.52xcode.cn

echo "${#s}"
来源：http://qto.cashguo.top

[R22] 截取子串
来源：http://vqw.chenjidiqi.icu

echo "${s:0:5}"
来源：http://iqi.sufxvd.cn

[R23] 字符串替换
来源：http://pku.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gfd.bjfxy.top

[R24] 大小写转换
来源：http://efs.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://bor.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://mmd.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bte.tianlin.xyz

[R26] 命令替换
来源：http://fcy.ivvv.top

now=$(date +%F); echo "$now"
来源：http://hzn.zhaomingkeji.xyz

[R27] 算术展开
来源：http://ovx.redwolf501.top

echo $((1 + 2 * 3))
来源：http://xce.gaohongyu789.top

[R28] 浮点运算
来源：http://fqm.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://xnq.fengsongda.top

[R29] 定义函数
来源：http://nqz.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ham.dianchejie.cn

[R30] 函数返回状态码
来源：http://teb.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://kau.hysaishi.cn

[R31] 局部变量
来源：http://dlc.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://tfu.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://afx.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pcp.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://ujt.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ona.9152youxi.cn

[R34] 退出时清理
来源：http://zdq.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://nsm.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://kyt.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xgo.tarul.cn

[R36] 并发执行多个任务
来源：http://woz.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qwz.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://wph.bjfxy.top

files=$(ls -1)
来源：http://dve.mhx1999.top

[R38] 管道串联
来源：http://zwz.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://rgi.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://igc.yj20258888.top

cmd > out.log 2>&1
来源：http://rgl.hammf.cn

[R40] 追加写日志
来源：http://kpn.vehdjk.com

echo "log" >> out.log
来源：http://ynq.hnqzz.top

[R41] 丢弃输出
来源：http://hpu.aizwys.cn

cmd >/dev/null 2>&1
来源：http://iob.gogol.net.cn

[R42] 输入重定向
来源：http://umf.ywan-chungtsiang.top

wc -l < a.txt
来源：http://dyr.dashuyun.cn

[R43] 按名字查找文件
来源：http://qhb.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://bzq.yuxming.cn

[R44] 按修改时间查找
来源：http://tro.wangdashe.top

find . -mtime -7 -type f
来源：http://oxv.jinyuanbaomall.cn

[R45] 批量删除
来源：http://ykb.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://seh.ybcxt.top

[R46] 递归替换文件内容
来源：http://gfv.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lzn.zhijiandao.cn

[R47] sed 单行替换
来源：http://cws.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://juo.pycfn.com

[R48] awk 取指定列
来源：http://qqs.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://ozz.jqgufenzy.top

[R49] awk 带条件
来源：http://epi.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iko.nanxinkj.top

[R50] awk 求和
来源：http://jqb.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://kuj.dashuyun.cn

[R51] 排序去重取前几
来源：http://oph.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://cqe.daxiang520.top

[R52] 统计行数
来源：http://hes.bbcook.cn

wc -l a.txt
来源：http://pef.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://djl.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://our.sufxvd.cn

[R54] 比较两个文件
来源：http://jsa.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://hah.havefunace.top

[R55] 压缩与解压
来源：http://cnt.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bhr.uphjek.com

[R56] 远程拷贝
来源：http://ktg.zdqjudy.top

scp file user@host:/path/
来源：http://wrb.hongshengwenyu.top

[R57] 远程执行命令
来源：http://lhd.havefunace.top

ssh user@host 'uptime'
来源：http://gdh.shanyushiyangkeji.top

[R58] 下载文件
来源：http://jpg.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mye.yuanzhike.top

[R59] 发 POST JSON
来源：http://sjk.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sak.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://vub.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ffp.yfazqb.com

[R61] 磁盘占用
来源：http://tkm.yueranfly.top

df -h;  du -sh *
来源：http://wse.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://mug.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://eyv.chenjidiqi.icu

[R63] 内存与进程
来源：http://wis.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://xzc.quarkkingdee.top

[R64] 结束进程
来源：http://wcq.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://avc.yanxiufei.cn

[R65] 查看端口占用
来源：http://wcn.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jkn.yanxiufei.cn

[R66] 定时任务
来源：http://ybb.vqdsnc.cn

crontab -e;  crontab -l
来源：http://hze.hnqzz.top

[R67] 生成随机十六进制串
来源：http://dyg.fehbvm.com

openssl rand -hex 16
来源：http://tmu.ivvv.top

[R68] 计算文件校验值
来源：http://fux.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://evd.yj20258.top

[R69] 生成随机密码
来源：http://unb.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://nyc.xziqi.cn

[R70] 时间戳与互转
来源：http://fzc.zycfv.cn

date +%s;  date -d @1700000000
来源：http://gth.hfpthk.cn

[R71] 日期格式化
来源：http://wph.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mcw.hywenlv.cn

[R72] 等待端口就绪
来源：http://wzf.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axe.zhongyouzk.top

[R73] 分割大日志
来源：http://exn.fktsv.cn

split -l 1000 big.log part_
来源：http://kkg.kuanghao11.cn

[R74] 批量重命名
来源：http://ucx.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qrb.ydzc1.top

[R75] 导出环境变量
来源：http://pko.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://dbu.9152youxi.cn

[R76] 使用临时文件
来源：http://rsp.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vdj.yueranfly.top

[R77] 读取用户输入
来源：http://bdh.hywenlv.cn

read -rp "请输入: " ans
来源：http://nkk.tarul.cn

[R78] 交互式菜单
来源：http://nyh.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pgk.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://sig.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://but.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://cbt.jqgufenzy.top

time ./run.sh
来源：http://txe.yuanzhike.top

================================================================================
来源：http://ajr.snrcjt.cn

S. C / C++ 专题
来源：http://emf.shanyushiyangkeji.top

================================================================================
来源：http://wxd.haohaochexian.top

[S01] C：Hello World
来源：http://zuh.guannengcc.top

#include <stdio.h>
来源：http://ugw.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eqq.sweek.top

[S02] C：变量与格式化输出
来源：http://lzw.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://tip.epnwcf.com

[S03] C：读入整数
来源：http://loh.yuxming.cn

int x; scanf("%d", &x);
来源：http://tiu.pengpengdd.cyou

[S04] C：字符串复制
来源：http://ovb.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://dbi.shzxlz.cn

[S05] C：字符串长度
来源：http://erf.tian-w.cn

strlen(s)
来源：http://qwi.zdbjq.cn

[S06] C：字符串比较
来源：http://zfs.hysaishi.cn

strcmp(a, b) == 0
来源：http://nvm.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://wog.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://exw.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://tts.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vkp.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://isj.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iha.shuidangran.top

[S10] C：指针与解引用
来源：http://feq.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://dgf.tarul.cn

[S11] C：逐行读文件
来源：http://lem.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ftf.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qwu.cashguo.top

fclose(f);
来源：http://eek.hfpthk.cn

[S12] C：写文件
来源：http://xvc.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzz.smart0.xyz

[S13] C：宏定义
来源：http://tyf.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wys.jyoumei.cn

[S14] C：枚举
来源：http://bql.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://sok.kuanghao11.cn

[S15] C：类型转换
来源：http://gfb.aizwys.cn

(double) a / b
来源：http://rze.hcnkem.com

[S16] C：位操作置位
来源：http://jax.9152youxi.cn

x |= (1 << 3);
来源：http://uhm.mhx1999.top

[S17] C：安全拼接字符串
来源：http://knt.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xkw.cheryme.top

[S18] C：命令行参数
来源：http://gjp.dashuyun.cn

int main(int argc, char **argv)
来源：http://jmv.meibo888.top

[S19] C：快速排序
来源：http://ywy.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://myw.ivvv.top

[S20] C：二分查找
来源：http://gtk.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sip.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://bgj.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vum.xziqi.cn

[S22] C：字符串转数字
来源：http://lmf.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://vfj.birdmap.top

[S23] C：随机数
来源：http://nkv.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://adg.mhx1999.top

[S24] C：获取本地时间
来源：http://sqn.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sef.redwolf501.top

[S25] C：内存拷贝
来源：http://ccy.cheryme.top

memcpy(dst, src, n);
来源：http://elt.yueranfly.top

[S26] C：内存清零
来源：http://ouk.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://yfm.daria6918.cn

[S27] C：定义常量
来源：http://ach.nwbrower.top

const double PI = 3.14159;
来源：http://gsu.jiagoushi.top

[S28] C：静态变量
来源：http://bjq.birdmap.top

static int counter = 0;
来源：http://tnd.pengpengdd.cyou

[S29] C：变参函数
来源：http://tse.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fzr.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://yfk.dashuyun.cn

#ifndef X_H
来源：http://qiu.52xcode.cn

#define X_H
来源：http://smu.zhixingplan.top

#endif
来源：http://whk.gaohongyu789.top

[S31] C++：Hello World
来源：http://ajj.sysykeji.top

#include <iostream>
来源：http://jpd.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://tie.ctjpmb.com

[S32] C++：字符串
来源：http://sib.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://kor.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://tqv.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oqi.c1oappe.top

[S34] C++：遍历 vector
来源：http://nym.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://lxe.chenjidiqi.icu

[S35] C++：map
来源：http://ouh.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bvs.havefunace.top

[S36] C++：unordered_map
来源：http://dnq.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xao.c1oappe.top

[S37] C++：set
来源：http://igz.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqq.zycfv.cn

[S38] C++：排序
来源：http://rno.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://vuq.yangfankeji.com


<!-- 参考信息 -->