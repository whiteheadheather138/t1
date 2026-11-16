代发 wailian999

[Q76] 按天统计
来源：http://imz.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xcr.jianghu66.top

[Q77] 时间加减
来源：http://mbn.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yjg.shangyingyoupin.top

[Q78] 当前时间
来源：http://fjr.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://axf.wangdashe.top

[Q79] 字符串拼接
来源：http://lnv.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lyx.birdmap.top

[Q80] 字符串截取
来源：http://ooy.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lyr.jqgufenzy.top

[Q81] 字符串替换
来源：http://cmm.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zcs.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://fnv.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eqe.svipenyu.cn

[Q83] 大小写转换
来源：http://ouy.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pmx.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://vsi.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://mvm.wangdashe.top

[Q85] 数值取整
来源：http://vlf.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://coq.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://qrd.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bpu.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://ovi.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vcw.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://fxh.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hpf.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ogx.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://nkc.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ynd.hysaishi.cn

[Q90] 生成序号列
来源：http://jgp.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbi.fktsv.cn

================================================================================
来源：http://fub.birdmap.top

R. Bash 专题
来源：http://ddd.yongpay.top

================================================================================
来源：http://djp.guannengcc.top

[R01] shebang 与严格模式
来源：http://shd.sjlbkw.cn

#!/usr/bin/env bash
来源：http://xdi.jqgfzy.top

set -euo pipefail
来源：http://ofm.sweek.top

[R02] 变量赋值与使用
来源：http://awr.sxryk.cn

name="Tom"; echo "$name"
来源：http://ppv.feifeiyinyue.top

[R03] 只读变量
来源：http://pli.aizwys.cn

readonly PI=3.14
来源：http://pxz.zhengqikj.top

[R04] 位置参数
来源：http://lbl.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jrr.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://aby.feifeiyinyue.top

name="${1:-default}"
来源：http://txm.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://gri.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jes.gaohongyu789.top

[R07] if 判断文件
来源：http://ayv.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dyv.yj20258888.top

[R08] 数值比较
来源：http://jia.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zyz.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://ico.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://znv.jlsjyb.cn

[R10] 正则匹配
来源：http://qpf.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ppg.fktsv.cn

[R11] case 多分支
来源：http://kkq.yuanzhike.top

case "$1" in
来源：http://kuf.xziqi.cn

start) echo "启动" ;;
来源：http://jyg.ybcxt.top

stop)  echo "停止" ;;
来源：http://qhb.meibo888.top

*)     echo "未知命令" ;;
来源：http://xut.jinqigfzy.top

esac
来源：http://mmg.gaohongyu789.top

[R12] for 遍历文件
来源：http://aev.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://aeh.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://dmp.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://dtc.yuxming.cn

[R14] C 风格 for
来源：http://mbq.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://joo.ybcxt.top

[R15] while 逐行读文件
来源：http://cmi.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://znm.epnwcf.com

[R16] until 等待条件
来源：http://lyv.tian-w.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gbv.andypj.xyz

[R17] 数组定义与取值
来源：http://msp.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yor.guowangkeji.top

[R18] 遍历数组
来源：http://gjj.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xwj.svipenyu.cn

[R19] 数组长度
来源：http://vxp.hnqzz.top

echo "${#arr[@]}"
来源：http://ssq.guannengcc.top

[R20] 关联数组（字典）
来源：http://xwe.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mnw.tarul.cn

[R21] 字符串长度
来源：http://bil.zhiwuduotai.top

echo "${#s}"
来源：http://klw.52xcode.cn

[R22] 截取子串
来源：http://udh.chenjidiqi.icu

echo "${s:0:5}"
来源：http://qpz.cashguo.top

[R23] 字符串替换
来源：http://aiq.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hmj.cashguo.top

[R24] 大小写转换
来源：http://rxr.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://opm.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://mny.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jxb.shanyushiyangkeji.top

[R26] 命令替换
来源：http://xat.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://kbw.gogol.net.cn

[R27] 算术展开
来源：http://hfi.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://zvz.jyoumei.cn

[R28] 浮点运算
来源：http://gnt.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://mpz.hcnkem.com

[R29] 定义函数
来源：http://gky.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mum.nwbrower.top

[R30] 函数返回状态码
来源：http://exx.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://cim.dashuyun.cn

[R31] 局部变量
来源：http://orm.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://mbe.zycfv.cn

[R32] 参数个数校验
来源：http://clw.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://drx.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://umm.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ywb.havefunace.top

[R34] 退出时清理
来源：http://auf.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jkq.redwolf501.top

[R35] 后台执行并等待
来源：http://nrr.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bwn.aizwys.cn

[R36] 并发执行多个任务
来源：http://yfo.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msd.cqqwz.cn

[R37] 把输出赋给变量
来源：http://fnl.zhixingplan.top

files=$(ls -1)
来源：http://ncg.yvedp.cn

[R38] 管道串联
来源：http://zii.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://kbs.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://rne.yuanzhike.top

cmd > out.log 2>&1
来源：http://eyq.tanke756.top

[R40] 追加写日志
来源：http://oeo.zdqjudy.top

echo "log" >> out.log
来源：http://hin.cqqwz.cn

[R41] 丢弃输出
来源：http://wii.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://uhn.vehdjk.com

[R42] 输入重定向
来源：http://egq.hcnkem.com

wc -l < a.txt
来源：http://czk.yj202588.top

[R43] 按名字查找文件
来源：http://azv.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://trw.sweek.top

[R44] 按修改时间查找
来源：http://gji.yj20258.top

find . -mtime -7 -type f
来源：http://slu.dianchejie.cn

[R45] 批量删除
来源：http://cvk.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://jxf.jianghu66.top

[R46] 递归替换文件内容
来源：http://aqp.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cge.andypj.xyz

[R47] sed 单行替换
来源：http://gad.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xyx.xuanzx.com

[R48] awk 取指定列
来源：http://xaj.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://bkn.fengsongda.top

[R49] awk 带条件
来源：http://rfy.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hkc.ybcxt.top

[R50] awk 求和
来源：http://jvd.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qbr.pycfn.com

[R51] 排序去重取前几
来源：http://jwp.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://paa.jyoumei.cn

[R52] 统计行数
来源：http://jnf.iojbl.cn

wc -l a.txt
来源：http://dvt.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://uzd.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gpg.redwolf501.top

[R54] 比较两个文件
来源：http://mqi.daria6918.cn

diff a.txt b.txt
来源：http://jlg.fehbvm.com

[R55] 压缩与解压
来源：http://zpv.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eom.ydjk.org.cn

[R56] 远程拷贝
来源：http://uhw.yongpay.top

scp file user@host:/path/
来源：http://ort.gogol.net.cn

[R57] 远程执行命令
来源：http://gfp.xinyue.icu

ssh user@host 'uptime'
来源：http://ucs.zdbjq.cn

[R58] 下载文件
来源：http://edq.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ver.yj202588.top

[R59] 发 POST JSON
来源：http://crb.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vbu.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://oky.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xoj.xuanzx.com

[R61] 磁盘占用
来源：http://yks.yonumen.top

df -h;  du -sh *
来源：http://msz.daxiang520.top

[R62] 找最占空间的文件
来源：http://jep.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://uwa.shzxlz.cn

[R63] 内存与进程
来源：http://abz.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://bka.yj20258888.top

[R64] 结束进程
来源：http://kip.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://ixy.fktsv.cn

[R65] 查看端口占用
来源：http://wym.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mjq.gogol.net.cn

[R66] 定时任务
来源：http://yij.dashuyun.cn

crontab -e;  crontab -l
来源：http://byu.sweek.top

[R67] 生成随机十六进制串
来源：http://atb.sxryk.cn

openssl rand -hex 16
来源：http://msq.uphjek.com

[R68] 计算文件校验值
来源：http://jtw.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yxx.vqdsnc.cn

[R69] 生成随机密码
来源：http://vxz.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://tje.cdnleiting.top

[R70] 时间戳与互转
来源：http://pnd.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://jaw.zhongyouzk.top

[R71] 日期格式化
来源：http://ytt.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kzt.epnwcf.com

[R72] 等待端口就绪
来源：http://xdv.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nsv.xuanzx.com

[R73] 分割大日志
来源：http://xbj.hnqzz.top

split -l 1000 big.log part_
来源：http://niz.ydzc1.top

[R74] 批量重命名
来源：http://gaj.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qtq.zhiwuduotai.top

[R75] 导出环境变量
来源：http://kzl.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://zjn.hcnkem.com

[R76] 使用临时文件
来源：http://rzm.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qdj.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://ypr.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://kxp.fzhhl.top

[R78] 交互式菜单
来源：http://nrp.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ggc.yfazqb.com

[R79] 解析命令行选项
来源：http://fce.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oez.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://zmr.xuanzx.com

time ./run.sh
来源：http://odw.meibo888.top

================================================================================
来源：http://rcs.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://nzm.jqgufenzy.top

================================================================================
来源：http://ibb.bbcook.cn

[S01] C：Hello World
来源：http://kyg.yonumen.top

#include <stdio.h>
来源：http://kre.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qha.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://xzq.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://xzs.zhiwuduotai.top

[S03] C：读入整数
来源：http://uxc.gzhubu.top

int x; scanf("%d", &x);
来源：http://nvl.wangshuangyany.cn

[S04] C：字符串复制
来源：http://lsj.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://uik.zdbjq.cn

[S05] C：字符串长度
来源：http://gbe.bjfxy.top

strlen(s)
来源：http://ezs.cucudq.cn

[S06] C：字符串比较
来源：http://eeb.jqgufenzy.top

strcmp(a, b) == 0
来源：http://ako.tarul.cn

[S07] C：数组遍历求和
来源：http://jfo.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mmk.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://zrk.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wac.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://fxh.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gfs.birdmap.top

[S10] C：指针与解引用
来源：http://kzf.epnwcf.com

int *p = &a;  *p = 5;
来源：http://rdi.svipenyu.cn

[S11] C：逐行读文件
来源：http://owl.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://ozb.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mjc.yj202588.top

fclose(f);
来源：http://cnl.birdmap.top

[S12] C：写文件
来源：http://ioc.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wvc.uphjek.com

[S13] C：宏定义
来源：http://ibk.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rpk.bbcook.cn

[S14] C：枚举
来源：http://tgk.wangshuangyany.cn

enum Color { RED, GREEN, BLUE };
来源：http://pqo.hywenlv.cn

[S15] C：类型转换
来源：http://qqh.andypj.xyz

(double) a / b
来源：http://tol.daria6918.cn

[S16] C：位操作置位
来源：http://pmn.316326.xyz

x |= (1 << 3);
来源：http://ome.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://hpp.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://koq.bbcook.cn

[S18] C：命令行参数
来源：http://zez.cdnleiting.top

int main(int argc, char **argv)
来源：http://kir.havefunace.top

[S19] C：快速排序
来源：http://psn.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://eax.yj20258888.top

[S20] C：二分查找
来源：http://ktq.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xig.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://gmz.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lrv.ehwqpu.com

[S22] C：字符串转数字
来源：http://txx.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://fos.chenjidiqi.icu

[S23] C：随机数
来源：http://uam.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ubt.yj20258888.top

[S24] C：获取本地时间
来源：http://qpd.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://swb.zhongyouzk.top

[S25] C：内存拷贝
来源：http://ada.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://cmm.svipenyu.cn

[S26] C：内存清零
来源：http://jdz.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://fak.jiagoushi.top

[S27] C：定义常量
来源：http://pwa.tianlin.xyz

const double PI = 3.14159;
来源：http://rnw.zhengqikj.top

[S28] C：静态变量
来源：http://zgs.sxryk.cn

static int counter = 0;
来源：http://buq.kuanghao11.cn

[S29] C：变参函数
来源：http://bmq.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://csq.quarkkingdee.top

[S30] C：头文件保护
来源：http://uss.ehwqpu.com

#ifndef X_H
来源：http://jbq.aizwys.cn

#define X_H
来源：http://xzl.9152youxi.cn

#endif
来源：http://lhr.hfpthk.cn

[S31] C++：Hello World
来源：http://xpq.wangshuangyany.cn

#include <iostream>
来源：http://rsh.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://sip.hcnkem.com

[S32] C++：字符串
来源：http://rao.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://izo.aizwys.cn

[S33] C++：vector 增删
来源：http://njd.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dgl.zhixingplan.top

[S34] C++：遍历 vector
来源：http://ccn.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://lyg.nwbrower.top

[S35] C++：map
来源：http://pxz.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rbo.gogol.net.cn

[S36] C++：unordered_map
来源：http://nva.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bju.vqdsnc.cn

[S37] C++：set
来源：http://yji.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://snt.hcnkem.com

[S38] C++：排序
来源：http://ykf.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://oyt.yonumen.top

[S39] C++：自定义比较器排序
来源：http://krd.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://afn.hnxiangtu.top

[S40] C++：查找元素
来源：http://zxu.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tgr.ctjpmb.com

[S41] C++：类与构造函数
来源：http://iot.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pei.tanke756.top

[S42] C++：继承与虚函数
来源：http://dfg.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://gpf.jlsjyb.cn

[S43] C++：智能指针
来源：http://kel.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://asg.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://thn.sysykeji.top

void inc(int &x) { ++x; }
来源：http://iyi.hammf.cn

[S45] C++：lambda
来源：http://yya.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://fkg.52xcode.cn

[S46] C++：函数模板
来源：http://rbm.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sqk.shzxlz.cn


<!-- 参考信息 -->