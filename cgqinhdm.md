代发 wailian999

[Q78] 当前时间
来源：http://uoi.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://snu.hysaishi.cn

[Q79] 字符串拼接
来源：http://tkt.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://osr.chenzaomai.com

[Q80] 字符串截取
来源：http://tup.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://scb.shuidangran.top

[Q81] 字符串替换
来源：http://kyf.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vxj.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://cgk.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tyg.nanxinkj.top

[Q83] 大小写转换
来源：http://wgu.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uae.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://dfn.xinyue.icu

SELECT TRIM(name) FROM users;
来源：http://zkm.daria6918.cn

[Q85] 数值取整
来源：http://gyq.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://amr.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://gvc.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aih.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://ydh.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yek.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://mje.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hxp.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ulf.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://ort.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pqq.c1oappe.top

[Q90] 生成序号列
来源：http://gbk.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cux.gotoacloud.top

================================================================================
来源：http://gkj.cashguo.top

R. Bash 专题
来源：http://qci.tarul.cn

================================================================================
来源：http://oxw.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://vit.bbcook.cn

#!/usr/bin/env bash
来源：http://ehs.meibo888.top

set -euo pipefail
来源：http://rlo.andypj.xyz

[R02] 变量赋值与使用
来源：http://jhq.gogol.net.cn

name="Tom"; echo "$name"
来源：http://gkz.zdbjq.cn

[R03] 只读变量
来源：http://lqt.zhaomingkeji.xyz

readonly PI=3.14
来源：http://ezw.snrcjt.cn

[R04] 位置参数
来源：http://dyv.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uls.ivvv.top

[R05] 参数默认值
来源：http://ffx.shuidangran.top

name="${1:-default}"
来源：http://jxr.aibaodan.cn

[R06] 判断命令是否存在
来源：http://cnw.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qiv.c1oappe.top

[R07] if 判断文件
来源：http://def.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nlt.yonumen.top

[R08] 数值比较
来源：http://ftn.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hed.yuxming.cn

[R09] 字符串比较
来源：http://jrf.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tzq.aizwys.cn

[R10] 正则匹配
来源：http://jkt.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rzn.andypj.xyz

[R11] case 多分支
来源：http://vzs.hcnkem.com

case "$1" in
来源：http://dkv.jiagoushi.top

start) echo "启动" ;;
来源：http://hne.mhx1999.top

stop)  echo "停止" ;;
来源：http://dag.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://wtq.gaohongyu789.top

esac
来源：http://mcb.yj20258.top

[R12] for 遍历文件
来源：http://imh.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://hlz.chenzaomai.com

[R13] for 计数循环
来源：http://yby.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://qdd.chenjidiqi.icu

[R14] C 风格 for
来源：http://reu.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sdi.iojbl.cn

[R15] while 逐行读文件
来源：http://tss.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ing.zhiwuduotai.top

[R16] until 等待条件
来源：http://wfm.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ics.jinqigufen.top

[R17] 数组定义与取值
来源：http://qrj.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://kyp.ydzc1.top

[R18] 遍历数组
来源：http://uhq.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nbn.xuanzx.com

[R19] 数组长度
来源：http://hye.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://ifb.aizwys.cn

[R20] 关联数组（字典）
来源：http://ufo.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kjx.guannengcc.top

[R21] 字符串长度
来源：http://ijn.zhiwuduotai.top

echo "${#s}"
来源：http://hzg.yj20258.top

[R22] 截取子串
来源：http://nmv.0kj1m.cn

echo "${s:0:5}"
来源：http://riv.hnxiangtu.top

[R23] 字符串替换
来源：http://dfa.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uoo.hammf.cn

[R24] 大小写转换
来源：http://rup.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://wup.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://cid.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://alk.52xcode.cn

[R26] 命令替换
来源：http://zdb.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://diw.9152youxi.cn

[R27] 算术展开
来源：http://zqy.yueranfly.top

echo $((1 + 2 * 3))
来源：http://zpo.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://kws.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://pwx.chenzaomai.com

[R29] 定义函数
来源：http://uyq.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yjv.sufxvd.cn

[R30] 函数返回状态码
来源：http://vvv.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://fzw.svipenyu.cn

[R31] 局部变量
来源：http://owh.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://omg.chenlongwang.top

[R32] 参数个数校验
来源：http://iml.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://khi.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://qrb.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ceo.52xcode.cn

[R34] 退出时清理
来源：http://dnz.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://sfj.sufxvd.cn

[R35] 后台执行并等待
来源：http://siu.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://avt.snrcjt.cn

[R36] 并发执行多个任务
来源：http://wlc.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vcn.yj20258888.top

[R37] 把输出赋给变量
来源：http://nvr.aibaodan.cn

files=$(ls -1)
来源：http://uzj.uphjek.com

[R38] 管道串联
来源：http://lxp.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://ipo.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://lnt.uphjek.com

cmd > out.log 2>&1
来源：http://prv.zycfv.cn

[R40] 追加写日志
来源：http://crh.cdnleiting.top

echo "log" >> out.log
来源：http://hqa.svipenyu.cn

[R41] 丢弃输出
来源：http://cwf.fzhhl.top

cmd >/dev/null 2>&1
来源：http://qec.gogol.net.cn

[R42] 输入重定向
来源：http://qzv.xuetiantiany.cn

wc -l < a.txt
来源：http://wps.bjfxy.top

[R43] 按名字查找文件
来源：http://ypl.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://iwk.cucudq.cn

[R44] 按修改时间查找
来源：http://gwr.zhijiandao.cn

find . -mtime -7 -type f
来源：http://vsh.chenjidiqi.icu

[R45] 批量删除
来源：http://rgg.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://cne.yfazqb.com

[R46] 递归替换文件内容
来源：http://nlb.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://svx.fehbvm.com

[R47] sed 单行替换
来源：http://mxa.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://zmj.tianlin.xyz

[R48] awk 取指定列
来源：http://ldn.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://fbp.sjlbkw.cn

[R49] awk 带条件
来源：http://yvn.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tmj.epnwcf.com

[R50] awk 求和
来源：http://ooh.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://bbn.andypj.xyz

[R51] 排序去重取前几
来源：http://jfp.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zwe.yanxiufei.cn

[R52] 统计行数
来源：http://ieo.chenjidiqi.icu

wc -l a.txt
来源：http://jrz.316326.xyz

[R53] 查看文件头与实时尾
来源：http://lid.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dxt.daria6918.cn

[R54] 比较两个文件
来源：http://pka.tarul.cn

diff a.txt b.txt
来源：http://kej.yangfankeji.com

[R55] 压缩与解压
来源：http://cru.yongpay.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bfz.hywenlv.cn

[R56] 远程拷贝
来源：http://eut.316326.xyz

scp file user@host:/path/
来源：http://wrt.ydjk.org.cn

[R57] 远程执行命令
来源：http://zac.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://fuj.hcnkem.com

[R58] 下载文件
来源：http://ygk.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xkq.havefunace.top

[R59] 发 POST JSON
来源：http://oqh.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eqf.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://rih.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yhz.jiagoushi.top

[R61] 磁盘占用
来源：http://gux.ehwqpu.com

df -h;  du -sh *
来源：http://lva.ivvv.top

[R62] 找最占空间的文件
来源：http://tfm.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://nyk.chenjidiqi.icu

[R63] 内存与进程
来源：http://rdj.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://kdm.shuidangran.top

[R64] 结束进程
来源：http://ewr.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://zeb.jqgfzy.top

[R65] 查看端口占用
来源：http://fyu.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yle.ehwqpu.com

[R66] 定时任务
来源：http://ubu.yongpay.top

crontab -e;  crontab -l
来源：http://ygu.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://stq.vqdsnc.cn

openssl rand -hex 16
来源：http://vhh.quarkkingdee.top

[R68] 计算文件校验值
来源：http://flb.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://wgb.tarul.cn

[R69] 生成随机密码
来源：http://bdc.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://tyj.zhongyouzk.top

[R70] 时间戳与互转
来源：http://mnh.fengsongda.top

date +%s;  date -d @1700000000
来源：http://voa.guowangkeji.top

[R71] 日期格式化
来源：http://kvs.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mem.xylfe.cn

[R72] 等待端口就绪
来源：http://lvy.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://xjd.aibaodan.cn

[R73] 分割大日志
来源：http://eqe.xinyue.icu

split -l 1000 big.log part_
来源：http://fzj.316326.xyz

[R74] 批量重命名
来源：http://eoo.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dal.yfazqb.com

[R75] 导出环境变量
来源：http://kju.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://pbg.shuidangran.top

[R76] 使用临时文件
来源：http://can.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://khr.yuxming.cn

[R77] 读取用户输入
来源：http://bpm.yangfankeji.com

read -rp "请输入: " ans
来源：http://cib.dianchejie.cn

[R78] 交互式菜单
来源：http://qku.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://tji.yonumen.top

[R79] 解析命令行选项
来源：http://uyt.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uwx.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://eui.tian-w.cn

time ./run.sh
来源：http://kmu.sxryk.cn

================================================================================
来源：http://afe.fzhhl.top

S. C / C++ 专题
来源：http://sdq.zhijiandao.cn

================================================================================
来源：http://otx.jinqigufen.top

[S01] C：Hello World
来源：http://pib.jlsjyb.cn

#include <stdio.h>
来源：http://ymt.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sbo.jianghu66.top

[S02] C：变量与格式化输出
来源：http://ydn.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://orf.mhx1999.top

[S03] C：读入整数
来源：http://kbz.smart0.xyz

int x; scanf("%d", &x);
来源：http://grh.vqdsnc.cn

[S04] C：字符串复制
来源：http://tvr.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://xwm.ydjk.org.cn

[S05] C：字符串长度
来源：http://nkz.daxiang520.top

strlen(s)
来源：http://phl.nanxuanxn.top

[S06] C：字符串比较
来源：http://cpy.bbcook.cn

strcmp(a, b) == 0
来源：http://ytr.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://lwa.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://umu.meibo888.top

[S08] C：动态内存分配与释放
来源：http://yyw.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://noz.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://svl.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xvg.zhijiandao.cn

[S10] C：指针与解引用
来源：http://zeh.hammf.cn

int *p = &a;  *p = 5;
来源：http://dbd.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://hph.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://ohr.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gcp.daria6918.cn

fclose(f);
来源：http://ird.xinyue.icu

[S12] C：写文件
来源：http://ciu.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://efl.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://alj.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qwq.nanxinkj.top

[S14] C：枚举
来源：http://brq.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://shs.cashguo.top

[S15] C：类型转换
来源：http://sis.cheryme.top

(double) a / b
来源：http://ojn.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://adg.yj20258.top

x |= (1 << 3);
来源：http://ijc.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://oxp.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hpc.vqdsnc.cn

[S18] C：命令行参数
来源：http://pje.dashuyun.cn

int main(int argc, char **argv)
来源：http://ohc.redwolf501.top

[S19] C：快速排序
来源：http://szp.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://vsn.ctjpmb.com

[S20] C：二分查找
来源：http://arb.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hjx.chenzaomai.com

[S21] C：字符类别判断
来源：http://yvc.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://spa.ppjwa.cn

[S22] C：字符串转数字
来源：http://wat.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://fkr.jlsjyb.cn

[S23] C：随机数
来源：http://mbj.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ksb.guannengcc.top

[S24] C：获取本地时间
来源：http://gpl.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gch.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://kuv.dianchejie.cn

memcpy(dst, src, n);
来源：http://hmr.xylfe.cn

[S26] C：内存清零
来源：http://jnc.bbcook.cn

memset(a, 0, sizeof a);
来源：http://psb.316326.xyz

[S27] C：定义常量
来源：http://bnb.svipenyu.cn

const double PI = 3.14159;
来源：http://sxk.tian-w.cn

[S28] C：静态变量
来源：http://suk.cucudq.cn

static int counter = 0;
来源：http://gcb.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://gwu.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lxh.ppjwa.cn

[S30] C：头文件保护
来源：http://hss.ydzc1.top

#ifndef X_H
来源：http://cig.sweek.top

#define X_H
来源：http://xad.jinyuanbaomall.cn

#endif
来源：http://yld.zhoulong.xyz

[S31] C++：Hello World
来源：http://rbw.nanxuanxn.top

#include <iostream>
来源：http://pus.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://dff.yongpay.top

[S32] C++：字符串
来源：http://hvx.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://wvj.zdqjudy.top

[S33] C++：vector 增删
来源：http://hzj.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dxj.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://ork.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://qfj.gotoacloud.top

[S35] C++：map
来源：http://lls.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xsi.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://qic.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yas.dashuyun.cn

[S37] C++：set
来源：http://crv.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bls.hesvh.cn

[S38] C++：排序
来源：http://cvl.yongpay.top

std::sort(v.begin(), v.end());
来源：http://bvm.yj20258.top

[S39] C++：自定义比较器排序
来源：http://tcj.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ocy.fehbvm.com

[S40] C++：查找元素
来源：http://nol.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cbm.hfpthk.cn

[S41] C++：类与构造函数
来源：http://omo.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rcr.hammf.cn

[S42] C++：继承与虚函数
来源：http://bxf.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://exi.snrcjt.cn

[S43] C++：智能指针
来源：http://gvm.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://kcp.yj20258.top

[S44] C++：引用传参
来源：http://jsc.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://rfh.haohaochexian.top

[S45] C++：lambda
来源：http://eas.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://uov.hnxiangtu.top

[S46] C++：函数模板
来源：http://qtv.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://slr.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://ehz.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ofa.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://hih.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://ldx.hammf.cn


<!-- 参考信息 -->