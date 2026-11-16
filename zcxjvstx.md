代发 wailian999

ANALYZE TABLE users;
来源：http://wmz.jyoumei.cn

[Q71] 查看建表语句
来源：http://kzu.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://adm.fengsongda.top

[Q72] 查看索引
来源：http://bis.shzxlz.cn

SHOW INDEX FROM users;
来源：http://frw.cheryme.top

[Q73] 查看表状态
来源：http://myj.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://rnl.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://nef.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zxe.tianlin.xyz

[Q75] 日期格式化
来源：http://zyv.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jpp.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rjf.yj20258888.top

[Q76] 按天统计
来源：http://ziw.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dtv.vqdsnc.cn

[Q77] 时间加减
来源：http://kmn.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eru.smart0.xyz

[Q78] 当前时间
来源：http://bod.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pyp.epnwcf.com

[Q79] 字符串拼接
来源：http://llv.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://soc.nanxinkj.top

[Q80] 字符串截取
来源：http://lnh.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rrv.52xcode.cn

[Q81] 字符串替换
来源：http://ehr.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cdi.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://iow.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bzu.svipenyu.cn

[Q83] 大小写转换
来源：http://rdz.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qhm.hfpthk.cn

[Q84] 去除首尾空格
来源：http://lhs.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://oga.redwolf501.top

[Q85] 数值取整
来源：http://xjv.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qvi.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://yhd.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iyj.yongpay.top

[Q87] JSON 字段做条件
来源：http://kms.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lyu.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://bkw.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://och.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxz.daxiang520.top

[Q89] 判断表是否存在
来源：http://llr.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lnc.hysaishi.cn

[Q90] 生成序号列
来源：http://yhp.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ufr.xuetiantiany.cn

================================================================================
来源：http://gwq.chenjidiqi.icu

R. Bash 专题
来源：http://hfj.yonumen.top

================================================================================
来源：http://ucw.hcnkem.com

[R01] shebang 与严格模式
来源：http://bmh.tarul.cn

#!/usr/bin/env bash
来源：http://nve.jyoumei.cn

set -euo pipefail
来源：http://pet.hammf.cn

[R02] 变量赋值与使用
来源：http://ruu.shuidangran.top

name="Tom"; echo "$name"
来源：http://qkt.shanyushiyangtech.top

[R03] 只读变量
来源：http://nmw.fanxiaobao.xyz

readonly PI=3.14
来源：http://vls.316326.xyz

[R04] 位置参数
来源：http://jpb.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kkc.zhijiandao.cn

[R05] 参数默认值
来源：http://jdr.andypj.xyz

name="${1:-default}"
来源：http://ydl.hammf.cn

[R06] 判断命令是否存在
来源：http://hkm.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hdk.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://xbh.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sps.pycfn.com

[R08] 数值比较
来源：http://bvv.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xon.ivvv.top

[R09] 字符串比较
来源：http://pgu.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tvg.svipenyu.cn

[R10] 正则匹配
来源：http://mbx.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://san.cucudq.cn

[R11] case 多分支
来源：http://xvn.sysykeji.top

case "$1" in
来源：http://znn.ehwqpu.com

start) echo "启动" ;;
来源：http://xgf.jianghu66.top

stop)  echo "停止" ;;
来源：http://wku.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://qjy.vehdjk.com

esac
来源：http://jti.ybcxt.top

[R12] for 遍历文件
来源：http://zsl.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://tlf.gaohongyu789.top

[R13] for 计数循环
来源：http://nrk.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://efr.feifeiyinyue.top

[R14] C 风格 for
来源：http://jtj.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lui.nanxuanxn.top

[R15] while 逐行读文件
来源：http://ktv.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sek.nanxuanxn.top

[R16] until 等待条件
来源：http://mqb.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hov.havefunace.top

[R17] 数组定义与取值
来源：http://zod.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://ked.nanxuanxn.top

[R18] 遍历数组
来源：http://tcg.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kjl.zhengqikj.top

[R19] 数组长度
来源：http://txy.vqdsnc.cn

echo "${#arr[@]}"
来源：http://qkq.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://yhe.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nza.nwbrower.top

[R21] 字符串长度
来源：http://ffz.smart0.xyz

echo "${#s}"
来源：http://uoi.pengpengdd.cyou

[R22] 截取子串
来源：http://rth.quarkkingdee.top

echo "${s:0:5}"
来源：http://czn.tanke756.top

[R23] 字符串替换
来源：http://dqy.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nee.ehwqpu.com

[R24] 大小写转换
来源：http://dqg.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://yxb.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://fjw.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ksj.fzhhl.top

[R26] 命令替换
来源：http://usm.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://zup.hammf.cn

[R27] 算术展开
来源：http://jyj.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://xqv.svipenyu.cn

[R28] 浮点运算
来源：http://dcx.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://adz.ehwqpu.com

[R29] 定义函数
来源：http://bbr.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baa.smart0.xyz

[R30] 函数返回状态码
来源：http://svr.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://qcb.tian-w.cn

[R31] 局部变量
来源：http://zzv.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://ojd.yanxiufei.cn

[R32] 参数个数校验
来源：http://dgs.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qwi.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://nqf.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hdx.jlsjyb.cn

[R34] 退出时清理
来源：http://wly.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xkg.jinqigfzy.top

[R35] 后台执行并等待
来源：http://flr.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yll.hfpthk.cn

[R36] 并发执行多个任务
来源：http://irj.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xnk.yvedp.cn

[R37] 把输出赋给变量
来源：http://fmm.yj20258888.top

files=$(ls -1)
来源：http://mhg.ivvv.top

[R38] 管道串联
来源：http://nfj.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://sky.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://ptq.dashuyun.cn

cmd > out.log 2>&1
来源：http://zsj.daria6918.cn

[R40] 追加写日志
来源：http://ruf.jqgufenzy.top

echo "log" >> out.log
来源：http://ett.hesvh.cn

[R41] 丢弃输出
来源：http://vyx.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://pec.mhx1999.top

[R42] 输入重定向
来源：http://cdi.jqgfzy.top

wc -l < a.txt
来源：http://soz.gzhubu.top

[R43] 按名字查找文件
来源：http://ede.vehdjk.com

find . -name "*.log" -type f
来源：http://muu.ehwqpu.com

[R44] 按修改时间查找
来源：http://dzx.yj20258.top

find . -mtime -7 -type f
来源：http://ucy.iojbl.cn

[R45] 批量删除
来源：http://ipf.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://prw.zhixingplan.top

[R46] 递归替换文件内容
来源：http://erb.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://szb.yj20258888.top

[R47] sed 单行替换
来源：http://tbw.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hxo.zhijiandao.cn

[R48] awk 取指定列
来源：http://ypp.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://omq.sxryk.cn

[R49] awk 带条件
来源：http://sck.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lbg.jiagoushi.top

[R50] awk 求和
来源：http://cwb.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://bug.dianchejie.cn

[R51] 排序去重取前几
来源：http://fgd.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://htz.yfazqb.com

[R52] 统计行数
来源：http://htl.shangyingyoupin.top

wc -l a.txt
来源：http://kgc.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://iyr.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wyp.xziqi.cn

[R54] 比较两个文件
来源：http://kwq.vqdsnc.cn

diff a.txt b.txt
来源：http://ouh.shangyingyoupin.top

[R55] 压缩与解压
来源：http://hdh.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zji.hfpthk.cn

[R56] 远程拷贝
来源：http://von.sweek.top

scp file user@host:/path/
来源：http://shn.snrcjt.cn

[R57] 远程执行命令
来源：http://nop.jlsjyb.cn

ssh user@host 'uptime'
来源：http://kgg.jinghuilouyu.cn

[R58] 下载文件
来源：http://ftn.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tfs.xuanzx.com

[R59] 发 POST JSON
来源：http://byc.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jub.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://tln.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bxr.fengsongda.top

[R61] 磁盘占用
来源：http://qjl.tianlin.xyz

df -h;  du -sh *
来源：http://iiq.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://oxu.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://zwy.chenlongwang.top

[R63] 内存与进程
来源：http://ddm.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://dud.yj20258888.top

[R64] 结束进程
来源：http://woe.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://xyf.nanxuanxn.top

[R65] 查看端口占用
来源：http://hzs.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dpk.xylfe.cn

[R66] 定时任务
来源：http://olw.zhixingplan.top

crontab -e;  crontab -l
来源：http://hon.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://ewx.ppjwa.cn

openssl rand -hex 16
来源：http://hvv.aibaodan.cn

[R68] 计算文件校验值
来源：http://dlp.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://ijb.sweek.top

[R69] 生成随机密码
来源：http://zzi.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://xdp.cashguo.top

[R70] 时间戳与互转
来源：http://kml.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://bbp.yuxming.cn

[R71] 日期格式化
来源：http://cbt.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qhb.yuxming.cn

[R72] 等待端口就绪
来源：http://xxp.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cbw.hesvh.cn

[R73] 分割大日志
来源：http://eya.fzhhl.top

split -l 1000 big.log part_
来源：http://usc.ctjpmb.com

[R74] 批量重命名
来源：http://mft.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zwv.yueranfly.top

[R75] 导出环境变量
来源：http://qid.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://kaq.dashuyun.cn

[R76] 使用临时文件
来源：http://oyo.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fub.cqqwz.cn

[R77] 读取用户输入
来源：http://ppm.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://aql.hesvh.cn

[R78] 交互式菜单
来源：http://brd.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dgp.yfazqb.com

[R79] 解析命令行选项
来源：http://nut.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pdw.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://svh.ivvv.top

time ./run.sh
来源：http://xof.iojbl.cn

================================================================================
来源：http://mjf.fehbvm.com

S. C / C++ 专题
来源：http://hwu.hnqzz.top

================================================================================
来源：http://cjy.hnqzz.top

[S01] C：Hello World
来源：http://gfx.xziqi.cn

#include <stdio.h>
来源：http://cvs.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xdp.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://uvq.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://fse.sxryk.cn

[S03] C：读入整数
来源：http://xrp.bjfxy.top

int x; scanf("%d", &x);
来源：http://wjw.jyoumei.cn

[S04] C：字符串复制
来源：http://ddu.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fnu.uphjek.com

[S05] C：字符串长度
来源：http://xwn.jiagoushi.top

strlen(s)
来源：http://cjm.xziqi.cn

[S06] C：字符串比较
来源：http://liw.sjlbkw.cn

strcmp(a, b) == 0
来源：http://emn.yuanzhike.top

[S07] C：数组遍历求和
来源：http://nvr.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jip.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://psz.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzf.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://rtw.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gci.jianghu66.top

[S10] C：指针与解引用
来源：http://gbk.andypj.xyz

int *p = &a;  *p = 5;
来源：http://dsa.birdmap.top

[S11] C：逐行读文件
来源：http://ptv.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://wxt.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ibq.andypj.xyz

fclose(f);
来源：http://usw.ywan-chungtsiang.top

[S12] C：写文件
来源：http://cgr.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nuz.feifeiyinyue.top

[S13] C：宏定义
来源：http://nhb.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dro.ywan-chungtsiang.top

[S14] C：枚举
来源：http://otp.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://mkx.pycfn.com

[S15] C：类型转换
来源：http://qiv.zhaomingkeji.xyz

(double) a / b
来源：http://tvl.gotoacloud.top

[S16] C：位操作置位
来源：http://qpu.ybcxt.top

x |= (1 << 3);
来源：http://vjx.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://xwf.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ffn.ppjwa.cn

[S18] C：命令行参数
来源：http://uni.hnqzz.top

int main(int argc, char **argv)
来源：http://zhr.shuidangran.top

[S19] C：快速排序
来源：http://abg.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://vaw.yueranfly.top

[S20] C：二分查找
来源：http://dxy.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lgz.yj20258888.top

[S21] C：字符类别判断
来源：http://irv.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xdp.ehwqpu.com

[S22] C：字符串转数字
来源：http://chp.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tek.hfpthk.cn

[S23] C：随机数
来源：http://cgm.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://klw.zhoulong.xyz

[S24] C：获取本地时间
来源：http://jva.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ssq.snrcjt.cn

[S25] C：内存拷贝
来源：http://djp.zhongyouzk.top

memcpy(dst, src, n);
来源：http://jvu.epnwcf.com

[S26] C：内存清零
来源：http://mnj.fengsongda.top

memset(a, 0, sizeof a);
来源：http://hnh.nanxuanxn.top

[S27] C：定义常量
来源：http://tdu.ppjwa.cn

const double PI = 3.14159;
来源：http://ghf.xinyue.icu

[S28] C：静态变量
来源：http://bkb.shanyushiyangtech.top

static int counter = 0;
来源：http://gdf.316326.xyz

[S29] C：变参函数
来源：http://cfz.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://csr.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://ucs.haohaochexian.top

#ifndef X_H
来源：http://kio.hnxiangtu.top

#define X_H
来源：http://maz.fzhhl.top

#endif
来源：http://yxn.bbcook.cn

[S31] C++：Hello World
来源：http://zgb.cqqwz.cn

#include <iostream>
来源：http://uve.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://fut.yonumen.top

[S32] C++：字符串
来源：http://ghz.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://nba.316326.xyz

[S33] C++：vector 增删
来源：http://dld.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ykr.yj202588.top

[S34] C++：遍历 vector
来源：http://vin.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://gln.guowangkeji.top

[S35] C++：map
来源：http://dlq.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://biw.hammf.cn

[S36] C++：unordered_map
来源：http://itu.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dmu.birdmap.top

[S37] C++：set
来源：http://xcv.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hlr.haohaochexian.top

[S38] C++：排序
来源：http://thn.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://rmt.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://tsd.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rwe.xuetiantiany.cn

[S40] C++：查找元素
来源：http://rzx.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mmi.yj20258888.top


<!-- 参考信息 -->