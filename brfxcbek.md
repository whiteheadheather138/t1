代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://adh.dianchejie.cn

[Q75] 日期格式化
来源：http://ttb.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ypf.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ztc.shzxlz.cn

[Q76] 按天统计
来源：http://lhl.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://voi.jyoumei.cn

[Q77] 时间加减
来源：http://mpf.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://itz.smart0.xyz

[Q78] 当前时间
来源：http://dsz.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wca.gaohongyu789.top

[Q79] 字符串拼接
来源：http://phf.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tbv.aibaodan.cn

[Q80] 字符串截取
来源：http://rjj.hcnkem.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wic.52xcode.cn

[Q81] 字符串替换
来源：http://vhq.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hob.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://wwn.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gfz.guowangkeji.top

[Q83] 大小写转换
来源：http://izo.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rso.daxiang520.top

[Q84] 去除首尾空格
来源：http://bdw.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://fxi.52xcode.cn

[Q85] 数值取整
来源：http://pvw.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lfp.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://tbn.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dzc.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://zls.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iol.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://thg.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vds.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uyc.yangfankeji.com

[Q89] 判断表是否存在
来源：http://xcu.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lwn.0kj1m.cn

[Q90] 生成序号列
来源：http://gby.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wak.zhengqikj.top

================================================================================
来源：http://alz.yvedp.cn

R. Bash 专题
来源：http://dro.nanxuanxn.top

================================================================================
来源：http://afl.yuxming.cn

[R01] shebang 与严格模式
来源：http://tfq.gaohongyu789.top

#!/usr/bin/env bash
来源：http://vsc.redwolf501.top

set -euo pipefail
来源：http://kub.ybcxt.top

[R02] 变量赋值与使用
来源：http://lmy.cucudq.cn

name="Tom"; echo "$name"
来源：http://pzm.hysaishi.cn

[R03] 只读变量
来源：http://ltj.jqgufenzy.top

readonly PI=3.14
来源：http://uxt.cqqwz.cn

[R04] 位置参数
来源：http://why.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ide.shzxlz.cn

[R05] 参数默认值
来源：http://ivd.smart0.xyz

name="${1:-default}"
来源：http://cok.hnqzz.top

[R06] 判断命令是否存在
来源：http://dvz.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mzq.yuxming.cn

[R07] if 判断文件
来源：http://qmf.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qeh.xziqi.cn

[R08] 数值比较
来源：http://qob.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sxv.havefunace.top

[R09] 字符串比较
来源：http://gcm.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uuv.0kj1m.cn

[R10] 正则匹配
来源：http://vra.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://faf.wangdashe.top

[R11] case 多分支
来源：http://cyq.hfpthk.cn

case "$1" in
来源：http://kjf.pycfn.com

start) echo "启动" ;;
来源：http://obk.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://jqi.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://tkp.ybcxt.top

esac
来源：http://dic.tanke756.top

[R12] for 遍历文件
来源：http://vxe.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://akb.hcnkem.com

[R13] for 计数循环
来源：http://hla.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://vwa.hcnkem.com

[R14] C 风格 for
来源：http://epc.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lew.cdnleiting.top

[R15] while 逐行读文件
来源：http://wea.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vim.ivvv.top

[R16] until 等待条件
来源：http://ais.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pgc.chenzaomai.com

[R17] 数组定义与取值
来源：http://igr.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qtv.ydzc1.top

[R18] 遍历数组
来源：http://bil.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://anq.daxiang520.top

[R19] 数组长度
来源：http://ydu.jiagoushi.top

echo "${#arr[@]}"
来源：http://hhz.ybcxt.top

[R20] 关联数组（字典）
来源：http://uqr.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lus.jlsjyb.cn

[R21] 字符串长度
来源：http://kjf.sysykeji.top

echo "${#s}"
来源：http://nzw.haohaochexian.top

[R22] 截取子串
来源：http://dfl.zhengqikj.top

echo "${s:0:5}"
来源：http://nsx.chenzaomai.com

[R23] 字符串替换
来源：http://gde.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nsr.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://eyu.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://utn.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://jez.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pwt.c1oappe.top

[R26] 命令替换
来源：http://gqk.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://wyg.jiagoushi.top

[R27] 算术展开
来源：http://ttr.uphjek.com

echo $((1 + 2 * 3))
来源：http://hfh.birdmap.top

[R28] 浮点运算
来源：http://yxx.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://nny.hnqzz.top

[R29] 定义函数
来源：http://qpg.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sgc.zdqjudy.top

[R30] 函数返回状态码
来源：http://blb.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://ktt.sufxvd.cn

[R31] 局部变量
来源：http://mze.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://may.kuanghao11.cn

[R32] 参数个数校验
来源：http://wqq.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fcx.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://ulg.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ozm.shanyushiyangtech.top

[R34] 退出时清理
来源：http://nfx.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://fkp.fengsongda.top

[R35] 后台执行并等待
来源：http://xes.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://epu.sxryk.cn

[R36] 并发执行多个任务
来源：http://bur.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hjb.iojbl.cn

[R37] 把输出赋给变量
来源：http://kdc.jinyuanbaomall.cn

files=$(ls -1)
来源：http://ssw.fanxiaobao.xyz

[R38] 管道串联
来源：http://bqk.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://pln.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://sug.xinyue.icu

cmd > out.log 2>&1
来源：http://qhg.fzhhl.top

[R40] 追加写日志
来源：http://tpx.chenjidiqi.icu

echo "log" >> out.log
来源：http://gvf.svipenyu.cn

[R41] 丢弃输出
来源：http://dwz.bjfxy.top

cmd >/dev/null 2>&1
来源：http://ein.yj202588.top

[R42] 输入重定向
来源：http://nmy.zdbjq.cn

wc -l < a.txt
来源：http://ara.havefunace.top

[R43] 按名字查找文件
来源：http://huf.jianghu66.top

find . -name "*.log" -type f
来源：http://vwg.epnwcf.com

[R44] 按修改时间查找
来源：http://tpq.316326.xyz

find . -mtime -7 -type f
来源：http://mlb.tianlin.xyz

[R45] 批量删除
来源：http://ysw.pycfn.com

find . -name "*.tmp" -delete
来源：http://rrv.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://kdq.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gor.tarul.cn

[R47] sed 单行替换
来源：http://nhp.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://wym.hongshengwenyu.top

[R48] awk 取指定列
来源：http://hwh.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://trt.hfpthk.cn

[R49] awk 带条件
来源：http://ina.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zvn.redwolf501.top

[R50] awk 求和
来源：http://jub.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://ybi.xuanzx.com

[R51] 排序去重取前几
来源：http://lyu.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hid.xuetiantiany.cn

[R52] 统计行数
来源：http://nhp.ivvv.top

wc -l a.txt
来源：http://pbb.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://psz.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xnq.meibo888.top

[R54] 比较两个文件
来源：http://kmj.quarkkingdee.top

diff a.txt b.txt
来源：http://pzk.c1oappe.top

[R55] 压缩与解压
来源：http://qvf.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://haq.sjlbkw.cn

[R56] 远程拷贝
来源：http://von.jinqigfzy.top

scp file user@host:/path/
来源：http://ejo.pengpengdd.cyou

[R57] 远程执行命令
来源：http://xdz.xylfe.cn

ssh user@host 'uptime'
来源：http://fwv.wangdashe.top

[R58] 下载文件
来源：http://wob.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ncv.cdnleiting.top

[R59] 发 POST JSON
来源：http://mvo.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pod.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://ikd.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fjh.yonumen.top

[R61] 磁盘占用
来源：http://egf.shuidangran.top

df -h;  du -sh *
来源：http://ejg.cucudq.cn

[R62] 找最占空间的文件
来源：http://ftb.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://ipe.316326.xyz

[R63] 内存与进程
来源：http://erl.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://qba.guannengcc.top

[R64] 结束进程
来源：http://oej.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://pcv.jinqigfzy.top

[R65] 查看端口占用
来源：http://jrq.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nfe.nwbrower.top

[R66] 定时任务
来源：http://wrw.yangfankeji.com

crontab -e;  crontab -l
来源：http://lts.shuidangran.top

[R67] 生成随机十六进制串
来源：http://ktp.nanxinkj.top

openssl rand -hex 16
来源：http://uyi.jqgfzy.top

[R68] 计算文件校验值
来源：http://xnf.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://nxb.zhengqikj.top

[R69] 生成随机密码
来源：http://rep.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://mhv.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://ywn.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://yru.yj20258.top

[R71] 日期格式化
来源：http://csz.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://weh.yonumen.top

[R72] 等待端口就绪
来源：http://glp.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oee.hfpthk.cn

[R73] 分割大日志
来源：http://sdl.meibo888.top

split -l 1000 big.log part_
来源：http://fvq.tarul.cn

[R74] 批量重命名
来源：http://eaw.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lnt.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://ckn.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://uzv.gzhubu.top

[R76] 使用临时文件
来源：http://qby.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://avo.ppjwa.cn

[R77] 读取用户输入
来源：http://jpv.yj20258.top

read -rp "请输入: " ans
来源：http://pwq.jiagoushi.top

[R78] 交互式菜单
来源：http://pvp.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oyb.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://yja.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rrl.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://kfs.yuanzhike.top

time ./run.sh
来源：http://uuj.zdbjq.cn

================================================================================
来源：http://ojk.0kj1m.cn

S. C / C++ 专题
来源：http://izz.aibaodan.cn

================================================================================
来源：http://vgy.tanke756.top

[S01] C：Hello World
来源：http://iou.yongpay.top

#include <stdio.h>
来源：http://suz.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dcz.fengsongda.top

[S02] C：变量与格式化输出
来源：http://tpi.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://dgq.tarul.cn

[S03] C：读入整数
来源：http://eoj.nanxinkj.top

int x; scanf("%d", &x);
来源：http://fee.kuanghao11.cn

[S04] C：字符串复制
来源：http://zqh.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://knd.jiagoushi.top

[S05] C：字符串长度
来源：http://kym.chenjidiqi.icu

strlen(s)
来源：http://pco.yj20258888.top

[S06] C：字符串比较
来源：http://lgl.zdqjudy.top

strcmp(a, b) == 0
来源：http://csz.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://udt.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tsn.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://uli.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lio.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://fmg.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rxc.cucudq.cn

[S10] C：指针与解引用
来源：http://wvh.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://mvt.cucudq.cn

[S11] C：逐行读文件
来源：http://ofy.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://bsv.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://goi.yonumen.top

fclose(f);
来源：http://ofq.ctjpmb.com

[S12] C：写文件
来源：http://sxl.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mvb.guowangkeji.top

[S13] C：宏定义
来源：http://fip.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fzl.chenzaomai.com

[S14] C：枚举
来源：http://cxf.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://ryq.chenlongwang.top

[S15] C：类型转换
来源：http://bkt.zhijiandao.cn

(double) a / b
来源：http://gun.vqdsnc.cn

[S16] C：位操作置位
来源：http://gni.hnqzz.top

x |= (1 << 3);
来源：http://esv.epnwcf.com

[S17] C：安全拼接字符串
来源：http://ftd.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ikw.xinyue.icu

[S18] C：命令行参数
来源：http://qjc.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://eug.xuanzx.com

[S19] C：快速排序
来源：http://oas.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://hhq.yj202588.top

[S20] C：二分查找
来源：http://uif.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cmx.guannengcc.top

[S21] C：字符类别判断
来源：http://hta.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rsd.shzxlz.cn

[S22] C：字符串转数字
来源：http://jnz.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://ywq.yfazqb.com

[S23] C：随机数
来源：http://zgc.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://ssv.fehbvm.com

[S24] C：获取本地时间
来源：http://hsv.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ezy.meibo888.top

[S25] C：内存拷贝
来源：http://kkm.hywenlv.cn

memcpy(dst, src, n);
来源：http://cnw.shzxlz.cn

[S26] C：内存清零
来源：http://lzj.xylfe.cn

memset(a, 0, sizeof a);
来源：http://csn.haohaochexian.top

[S27] C：定义常量
来源：http://pbn.yonumen.top

const double PI = 3.14159;
来源：http://uhg.sysykeji.top

[S28] C：静态变量
来源：http://sin.zdbjq.cn

static int counter = 0;
来源：http://shb.wangshuangyany.cn

[S29] C：变参函数
来源：http://okq.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fzp.epnwcf.com

[S30] C：头文件保护
来源：http://qzm.sweek.top

#ifndef X_H
来源：http://iiy.hongshengwenyu.top

#define X_H
来源：http://lck.0kj1m.cn

#endif
来源：http://qyi.nanxuanxn.top

[S31] C++：Hello World
来源：http://zvm.0kj1m.cn

#include <iostream>
来源：http://scb.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://qlh.sysykeji.top

[S32] C++：字符串
来源：http://fur.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://zfa.vqdsnc.cn

[S33] C++：vector 增删
来源：http://mzz.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gjf.zycfv.cn

[S34] C++：遍历 vector
来源：http://ciu.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://oen.bjfxy.top

[S35] C++：map
来源：http://usx.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fip.yongpay.top

[S36] C++：unordered_map
来源：http://prx.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gjy.jinyuanbaomall.cn

[S37] C++：set
来源：http://zwk.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://szw.birdmap.top

[S38] C++：排序
来源：http://mpe.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://bkw.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://xuv.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bob.andypj.xyz

[S40] C++：查找元素
来源：http://rpg.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yni.hywenlv.cn

[S41] C++：类与构造函数
来源：http://bbg.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwe.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://smn.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://qia.guowangkeji.top

[S43] C++：智能指针
来源：http://mts.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://pri.gotoacloud.top

[S44] C++：引用传参
来源：http://mbb.meibo888.top

void inc(int &x) { ++x; }
来源：http://kba.smart0.xyz


<!-- 参考信息 -->