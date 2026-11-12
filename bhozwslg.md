代发 wailian999

[Q76] 按天统计
来源：http://ybm.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rsp.ydzc1.top

[Q77] 时间加减
来源：http://klc.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fry.hcnkem.com

[Q78] 当前时间
来源：http://usc.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wqh.yvedp.cn

[Q79] 字符串拼接
来源：http://bij.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jwr.yuanzhike.top

[Q80] 字符串截取
来源：http://wrt.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hcr.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://ifm.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://phd.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://ehv.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ecq.fehbvm.com

[Q83] 大小写转换
来源：http://qtq.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yqp.andypj.xyz

[Q84] 去除首尾空格
来源：http://ejr.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://syl.yj20258888.top

[Q85] 数值取整
来源：http://gzt.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qwj.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://ibw.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zgq.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://fbw.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lrc.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://lgm.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://buz.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zjh.snrcjt.cn

[Q89] 判断表是否存在
来源：http://ueo.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eyl.sweek.top

[Q90] 生成序号列
来源：http://jnf.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dln.smart0.xyz

================================================================================
来源：http://cif.jyoumei.cn

R. Bash 专题
来源：http://gig.shuidangran.top

================================================================================
来源：http://vqe.0kj1m.cn

[R01] shebang 与严格模式
来源：http://wzn.zycfv.cn

#!/usr/bin/env bash
来源：http://owa.nanxinkj.top

set -euo pipefail
来源：http://kln.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://pzl.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://reb.hnxiangtu.top

[R03] 只读变量
来源：http://sfr.ivvv.top

readonly PI=3.14
来源：http://lxt.xuanzx.com

[R04] 位置参数
来源：http://rgg.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jvv.sxryk.cn

[R05] 参数默认值
来源：http://ycl.yj20258.top

name="${1:-default}"
来源：http://xzn.chenzaomai.com

[R06] 判断命令是否存在
来源：http://uuw.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pkz.fzhhl.top

[R07] if 判断文件
来源：http://hyq.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fer.chenzaomai.com

[R08] 数值比较
来源：http://bgy.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nbe.hywenlv.cn

[R09] 字符串比较
来源：http://bpy.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zmu.yueranfly.top

[R10] 正则匹配
来源：http://ayf.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vum.yuxming.cn

[R11] case 多分支
来源：http://ulj.guowangkeji.top

case "$1" in
来源：http://dgs.tianlin.xyz

start) echo "启动" ;;
来源：http://zjz.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://kvc.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://ugm.haohaochexian.top

esac
来源：http://sjy.0kj1m.cn

[R12] for 遍历文件
来源：http://gfv.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://tsu.ydjk.org.cn

[R13] for 计数循环
来源：http://jjr.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://jmn.pycfn.com

[R14] C 风格 for
来源：http://gwe.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bcm.daxiang520.top

[R15] while 逐行读文件
来源：http://syz.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ovn.zhengqikj.top

[R16] until 等待条件
来源：http://mlr.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xnp.hesvh.cn

[R17] 数组定义与取值
来源：http://dhy.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://fai.ctjpmb.com

[R18] 遍历数组
来源：http://qzo.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nqz.zhongyouzk.top

[R19] 数组长度
来源：http://fvd.iojbl.cn

echo "${#arr[@]}"
来源：http://frb.ehwqpu.com

[R20] 关联数组（字典）
来源：http://mgy.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zby.hammf.cn

[R21] 字符串长度
来源：http://vxl.sjlbkw.cn

echo "${#s}"
来源：http://mcg.sufxvd.cn

[R22] 截取子串
来源：http://sqa.yvedp.cn

echo "${s:0:5}"
来源：http://jrd.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://epr.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gvy.tarul.cn

[R24] 大小写转换
来源：http://ezh.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rqz.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://voh.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zwy.xinyue.icu

[R26] 命令替换
来源：http://frr.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://kzg.yvedp.cn

[R27] 算术展开
来源：http://hyr.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://jni.cdnleiting.top

[R28] 浮点运算
来源：http://mcl.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://nxr.zhoulong.xyz

[R29] 定义函数
来源：http://umc.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bgs.nanxinkj.top

[R30] 函数返回状态码
来源：http://fam.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://snx.9152youxi.cn

[R31] 局部变量
来源：http://wdi.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://otl.daria6918.cn

[R32] 参数个数校验
来源：http://kbd.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gaa.sweek.top

[R33] 捕获错误并提示行号
来源：http://wla.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://skh.smart0.xyz

[R34] 退出时清理
来源：http://jot.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lvs.xylfe.cn

[R35] 后台执行并等待
来源：http://yoz.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://suo.yueranfly.top

[R36] 并发执行多个任务
来源：http://zet.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mvz.ppjwa.cn

[R37] 把输出赋给变量
来源：http://yqe.ydjk.org.cn

files=$(ls -1)
来源：http://ozi.yangfankeji.com

[R38] 管道串联
来源：http://hyv.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://wsd.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://ubb.316326.xyz

cmd > out.log 2>&1
来源：http://cul.gogol.net.cn

[R40] 追加写日志
来源：http://ern.tianlin.xyz

echo "log" >> out.log
来源：http://tyj.hongshengwenyu.top

[R41] 丢弃输出
来源：http://iiq.hesvh.cn

cmd >/dev/null 2>&1
来源：http://nvt.cdnleiting.top

[R42] 输入重定向
来源：http://psf.bbcook.cn

wc -l < a.txt
来源：http://nsh.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://ztf.sufxvd.cn

find . -name "*.log" -type f
来源：http://xuh.jlsjyb.cn

[R44] 按修改时间查找
来源：http://ocu.ehwqpu.com

find . -mtime -7 -type f
来源：http://zae.zhengqikj.top

[R45] 批量删除
来源：http://snp.wangdashe.top

find . -name "*.tmp" -delete
来源：http://bju.guannengcc.top

[R46] 递归替换文件内容
来源：http://pqd.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sso.shangyingyoupin.top

[R47] sed 单行替换
来源：http://sst.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://act.hongshengwenyu.top

[R48] awk 取指定列
来源：http://nam.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://ntr.chenjidiqi.icu

[R49] awk 带条件
来源：http://hwu.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sqo.redwolf501.top

[R50] awk 求和
来源：http://mgp.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://iic.daria6918.cn

[R51] 排序去重取前几
来源：http://gtf.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bgo.jinqigfzy.top

[R52] 统计行数
来源：http://azj.dashuyun.cn

wc -l a.txt
来源：http://xrq.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://grd.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nrp.jinqigfzy.top

[R54] 比较两个文件
来源：http://jcq.hammf.cn

diff a.txt b.txt
来源：http://gzf.dashuyun.cn

[R55] 压缩与解压
来源：http://tmg.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jqa.jqgufenzy.top

[R56] 远程拷贝
来源：http://ffv.mhx1999.top

scp file user@host:/path/
来源：http://hxa.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://val.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://dqq.ivvv.top

[R58] 下载文件
来源：http://gyl.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ukq.svipenyu.cn

[R59] 发 POST JSON
来源：http://psg.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yow.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://hge.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uda.gaohongyu789.top

[R61] 磁盘占用
来源：http://fnu.havefunace.top

df -h;  du -sh *
来源：http://vsd.gogol.net.cn

[R62] 找最占空间的文件
来源：http://puw.birdmap.top

du -ah . | sort -rh | head -10
来源：http://vuu.zhengqikj.top

[R63] 内存与进程
来源：http://hqs.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://fyf.ivvv.top

[R64] 结束进程
来源：http://bco.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://cub.sysykeji.top

[R65] 查看端口占用
来源：http://msq.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kfi.tian-w.cn

[R66] 定时任务
来源：http://rxg.fehbvm.com

crontab -e;  crontab -l
来源：http://arj.fzhhl.top

[R67] 生成随机十六进制串
来源：http://urk.bbcook.cn

openssl rand -hex 16
来源：http://cki.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://wgs.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vkk.svipenyu.cn

[R69] 生成随机密码
来源：http://ige.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://edx.uphjek.com

[R70] 时间戳与互转
来源：http://shi.cashguo.top

date +%s;  date -d @1700000000
来源：http://hyj.epnwcf.com

[R71] 日期格式化
来源：http://ydx.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ouu.zdbjq.cn

[R72] 等待端口就绪
来源：http://lts.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jbh.ppjwa.cn

[R73] 分割大日志
来源：http://nvm.ctjpmb.com

split -l 1000 big.log part_
来源：http://eyz.yuxming.cn

[R74] 批量重命名
来源：http://thz.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqm.zycfv.cn

[R75] 导出环境变量
来源：http://wbx.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://vet.gotoacloud.top

[R76] 使用临时文件
来源：http://bft.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zyu.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://fok.quarkkingdee.top

read -rp "请输入: " ans
来源：http://reh.andypj.xyz

[R78] 交互式菜单
来源：http://uck.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mxm.xylfe.cn

[R79] 解析命令行选项
来源：http://ylu.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hrm.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://uyq.jlsjyb.cn

time ./run.sh
来源：http://sbs.ivvv.top

================================================================================
来源：http://eyy.9152youxi.cn

S. C / C++ 专题
来源：http://yir.havefunace.top

================================================================================
来源：http://uuq.52xcode.cn

[S01] C：Hello World
来源：http://psh.vqdsnc.cn

#include <stdio.h>
来源：http://tzg.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://rmf.havefunace.top

[S02] C：变量与格式化输出
来源：http://ewh.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://zli.cucudq.cn

[S03] C：读入整数
来源：http://dhb.fzhhl.top

int x; scanf("%d", &x);
来源：http://bbs.wangdashe.top

[S04] C：字符串复制
来源：http://fua.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oiz.jqgfzy.top

[S05] C：字符串长度
来源：http://cyt.pengpengdd.cyou

strlen(s)
来源：http://zln.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://blj.cheryme.top

strcmp(a, b) == 0
来源：http://ejy.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://lpl.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qro.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://fui.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://obe.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://aoh.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jpd.sxryk.cn

[S10] C：指针与解引用
来源：http://bga.cheryme.top

int *p = &a;  *p = 5;
来源：http://aap.zdqjudy.top

[S11] C：逐行读文件
来源：http://nlx.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://uks.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yqt.pycfn.com

fclose(f);
来源：http://xav.feifeiyinyue.top

[S12] C：写文件
来源：http://cny.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jon.zycfv.cn

[S13] C：宏定义
来源：http://cxj.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucm.jqgfzy.top

[S14] C：枚举
来源：http://yev.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://gdd.vqdsnc.cn

[S15] C：类型转换
来源：http://cvh.jianghu66.top

(double) a / b
来源：http://jvd.yfazqb.com

[S16] C：位操作置位
来源：http://imb.hesvh.cn

x |= (1 << 3);
来源：http://lcu.fehbvm.com

[S17] C：安全拼接字符串
来源：http://nkp.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eww.yuxming.cn

[S18] C：命令行参数
来源：http://qjd.jiagoushi.top

int main(int argc, char **argv)
来源：http://rui.fktsv.cn

[S19] C：快速排序
来源：http://fnb.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://ppm.jyoumei.cn

[S20] C：二分查找
来源：http://gwu.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://upx.dianchejie.cn

[S21] C：字符类别判断
来源：http://gyg.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://key.c1oappe.top

[S22] C：字符串转数字
来源：http://uuj.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://mwu.mhx1999.top

[S23] C：随机数
来源：http://qwo.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eop.ivvv.top

[S24] C：获取本地时间
来源：http://ypy.vehdjk.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wvr.zhijiandao.cn

[S25] C：内存拷贝
来源：http://jkp.haohaochexian.top

memcpy(dst, src, n);
来源：http://itt.hfpthk.cn

[S26] C：内存清零
来源：http://gbd.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://pxy.jianghu66.top

[S27] C：定义常量
来源：http://hzr.ybcxt.top

const double PI = 3.14159;
来源：http://jmw.yangfankeji.com

[S28] C：静态变量
来源：http://nyr.yuxming.cn

static int counter = 0;
来源：http://ocg.meibo888.top

[S29] C：变参函数
来源：http://ifk.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hly.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://tlk.wangshuangyany.cn

#ifndef X_H
来源：http://wkq.zhijiandao.cn

#define X_H
来源：http://jsj.hesvh.cn

#endif
来源：http://yrx.aizwys.cn

[S31] C++：Hello World
来源：http://kgc.smart0.xyz

#include <iostream>
来源：http://tsa.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://nvv.cashguo.top

[S32] C++：字符串
来源：http://hue.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://lsu.ppjwa.cn

[S33] C++：vector 增删
来源：http://sjx.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gmh.birdmap.top

[S34] C++：遍历 vector
来源：http://oxd.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://yul.shanyushiyangkeji.top

[S35] C++：map
来源：http://gop.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pgo.fengsongda.top

[S36] C++：unordered_map
来源：http://szh.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vaw.hfpthk.cn

[S37] C++：set
来源：http://rqw.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cxz.c1oappe.top

[S38] C++：排序
来源：http://esy.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://cbv.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://ald.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ihe.jqgufenzy.top

[S40] C++：查找元素
来源：http://lvi.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tcl.cheryme.top

[S41] C++：类与构造函数
来源：http://mwh.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ihn.andypj.xyz

[S42] C++：继承与虚函数
来源：http://xko.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://ejm.jyoumei.cn

[S43] C++：智能指针
来源：http://gkx.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://his.yj20258888.top

[S44] C++：引用传参
来源：http://ala.yuxming.cn

void inc(int &x) { ++x; }
来源：http://wyi.zhengqikj.top

[S45] C++：lambda
来源：http://zqj.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://nkz.zhiwuduotai.top

[S46] C++：函数模板
来源：http://tcf.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mbu.fehbvm.com


<!-- 参考信息 -->