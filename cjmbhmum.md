代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zch.yongpay.top

[Q75] 日期格式化
来源：http://nde.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fyt.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://veh.hnxiangtu.top

[Q76] 按天统计
来源：http://uvx.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uzt.jqgufenzy.top

[Q77] 时间加减
来源：http://fpj.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eme.ctjpmb.com

[Q78] 当前时间
来源：http://kmf.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bqg.zhongyouzk.top

[Q79] 字符串拼接
来源：http://fmi.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://maw.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://xwj.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iug.yj20258888.top

[Q81] 字符串替换
来源：http://zqd.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rrz.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://tsd.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gcu.jyoumei.cn

[Q83] 大小写转换
来源：http://zss.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jjz.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://wke.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://clf.yj20258.top

[Q85] 数值取整
来源：http://acp.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvc.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://axz.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ksc.tanke756.top

[Q87] JSON 字段做条件
来源：http://aqt.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gta.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://gzw.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nlq.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ecb.jqgfzy.top

[Q89] 判断表是否存在
来源：http://vxu.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qus.smart0.xyz

[Q90] 生成序号列
来源：http://qev.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hxq.zhongyouzk.top

================================================================================
来源：http://yik.dashuyun.cn

R. Bash 专题
来源：http://loa.hesvh.cn

================================================================================
来源：http://yen.pycfn.com

[R01] shebang 与严格模式
来源：http://cas.zdqjudy.top

#!/usr/bin/env bash
来源：http://fem.tanke756.top

set -euo pipefail
来源：http://uim.yvedp.cn

[R02] 变量赋值与使用
来源：http://gkp.cucudq.cn

name="Tom"; echo "$name"
来源：http://vnm.shanyushiyangkeji.top

[R03] 只读变量
来源：http://xez.hongshengwenyu.top

readonly PI=3.14
来源：http://vrj.epnwcf.com

[R04] 位置参数
来源：http://vtr.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://acj.ivvv.top

[R05] 参数默认值
来源：http://goy.xylfe.cn

name="${1:-default}"
来源：http://iom.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://wfy.xylfe.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xmp.havefunace.top

[R07] if 判断文件
来源：http://ejc.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fzw.zhaomingkeji.xyz

[R08] 数值比较
来源：http://xri.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zbu.zhengqikj.top

[R09] 字符串比较
来源：http://bmh.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bfd.52xcode.cn

[R10] 正则匹配
来源：http://lcd.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://imc.yj20258888.top

[R11] case 多分支
来源：http://afi.hesvh.cn

case "$1" in
来源：http://khf.yueranfly.top

start) echo "启动" ;;
来源：http://nnb.daria6918.cn

stop)  echo "停止" ;;
来源：http://euy.smart0.xyz

*)     echo "未知命令" ;;
来源：http://hwp.gaohongyu789.top

esac
来源：http://gvb.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://nrb.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://uqo.andypj.xyz

[R13] for 计数循环
来源：http://ivw.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://xap.ydjk.org.cn

[R14] C 风格 for
来源：http://raz.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ote.fehbvm.com

[R15] while 逐行读文件
来源：http://mjn.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oxu.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://jnu.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nne.yuxming.cn

[R17] 数组定义与取值
来源：http://ngc.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://kos.jinghuilouyu.cn

[R18] 遍历数组
来源：http://jdc.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ocn.jqgufenzy.top

[R19] 数组长度
来源：http://lvr.pycfn.com

echo "${#arr[@]}"
来源：http://gxb.hnqzz.top

[R20] 关联数组（字典）
来源：http://pyb.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dqj.jinghuilouyu.cn

[R21] 字符串长度
来源：http://omw.yvedp.cn

echo "${#s}"
来源：http://hdq.ppjwa.cn

[R22] 截取子串
来源：http://wxi.aizwys.cn

echo "${s:0:5}"
来源：http://tix.ydzc1.top

[R23] 字符串替换
来源：http://gnt.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfw.cheryme.top

[R24] 大小写转换
来源：http://wky.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hpq.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://fjm.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nhe.wangdashe.top

[R26] 命令替换
来源：http://uks.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://ycu.c1oappe.top

[R27] 算术展开
来源：http://xvh.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://xck.gogol.net.cn

[R28] 浮点运算
来源：http://thp.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://ufm.cucudq.cn

[R29] 定义函数
来源：http://ssh.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bos.cashguo.top

[R30] 函数返回状态码
来源：http://sdn.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://ife.haohaochexian.top

[R31] 局部变量
来源：http://rnr.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://fde.316326.xyz

[R32] 参数个数校验
来源：http://krg.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dgf.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://exz.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gie.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://vya.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://rda.fzhhl.top

[R35] 后台执行并等待
来源：http://bkj.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jxi.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://bzi.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xwj.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://awy.0kj1m.cn

files=$(ls -1)
来源：http://zsg.kuanghao11.cn

[R38] 管道串联
来源：http://bjl.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://eqw.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://vtp.hammf.cn

cmd > out.log 2>&1
来源：http://avs.zhongyouzk.top

[R40] 追加写日志
来源：http://eko.feifeiyinyue.top

echo "log" >> out.log
来源：http://qzc.fktsv.cn

[R41] 丢弃输出
来源：http://kya.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://uxf.kuanghao11.cn

[R42] 输入重定向
来源：http://erq.xuetiantiany.cn

wc -l < a.txt
来源：http://uyq.guowangkeji.top

[R43] 按名字查找文件
来源：http://cue.svipenyu.cn

find . -name "*.log" -type f
来源：http://hvk.cheryme.top

[R44] 按修改时间查找
来源：http://wru.hcnkem.com

find . -mtime -7 -type f
来源：http://phf.yueranfly.top

[R45] 批量删除
来源：http://uul.shuidangran.top

find . -name "*.tmp" -delete
来源：http://kfj.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://rll.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hga.daxiang520.top

[R47] sed 单行替换
来源：http://hvg.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://kta.hcnkem.com

[R48] awk 取指定列
来源：http://voc.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://bag.xuanzx.com

[R49] awk 带条件
来源：http://zbz.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qwq.wangshuangyany.cn

[R50] awk 求和
来源：http://rxv.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kvr.tarul.cn

[R51] 排序去重取前几
来源：http://lnf.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qzm.zhengqikj.top

[R52] 统计行数
来源：http://ijr.guannengcc.top

wc -l a.txt
来源：http://kzs.hammf.cn

[R53] 查看文件头与实时尾
来源：http://bne.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xug.daria6918.cn

[R54] 比较两个文件
来源：http://ulu.shzxlz.cn

diff a.txt b.txt
来源：http://kzm.sxryk.cn

[R55] 压缩与解压
来源：http://xcn.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rls.yvedp.cn

[R56] 远程拷贝
来源：http://kns.jinqigufen.top

scp file user@host:/path/
来源：http://shh.shangyingyoupin.top

[R57] 远程执行命令
来源：http://syv.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://xii.chenjidiqi.icu

[R58] 下载文件
来源：http://sit.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://heb.guowangkeji.top

[R59] 发 POST JSON
来源：http://uyo.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lkb.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://vvn.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tcp.haohaochexian.top

[R61] 磁盘占用
来源：http://htw.chenzaomai.com

df -h;  du -sh *
来源：http://wwf.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://jqc.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://kxn.epnwcf.com

[R63] 内存与进程
来源：http://cfr.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://lcd.fehbvm.com

[R64] 结束进程
来源：http://zen.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://plj.hfpthk.cn

[R65] 查看端口占用
来源：http://opb.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://afy.tarul.cn

[R66] 定时任务
来源：http://smz.epnwcf.com

crontab -e;  crontab -l
来源：http://bny.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://cnk.hesvh.cn

openssl rand -hex 16
来源：http://noq.zhixingplan.top

[R68] 计算文件校验值
来源：http://zea.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://lna.zhijiandao.cn

[R69] 生成随机密码
来源：http://sii.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://ljj.hcnkem.com

[R70] 时间戳与互转
来源：http://jui.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://ila.yfazqb.com

[R71] 日期格式化
来源：http://yup.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uwn.fzhhl.top

[R72] 等待端口就绪
来源：http://bsv.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jih.birdmap.top

[R73] 分割大日志
来源：http://doy.jqgfzy.top

split -l 1000 big.log part_
来源：http://ada.gogol.net.cn

[R74] 批量重命名
来源：http://hbu.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://reu.cdnleiting.top

[R75] 导出环境变量
来源：http://pwj.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://iyh.ppjwa.cn

[R76] 使用临时文件
来源：http://smx.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mbf.guowangkeji.top

[R77] 读取用户输入
来源：http://tqe.ybcxt.top

read -rp "请输入: " ans
来源：http://mtr.fengsongda.top

[R78] 交互式菜单
来源：http://kgc.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qik.zhoulong.xyz

[R79] 解析命令行选项
来源：http://pdd.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iaf.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://btx.shanyushiyangtech.top

time ./run.sh
来源：http://iwo.svipenyu.cn

================================================================================
来源：http://roy.dashuyun.cn

S. C / C++ 专题
来源：http://ady.daria6918.cn

================================================================================
来源：http://zqq.hysaishi.cn

[S01] C：Hello World
来源：http://zyy.yfazqb.com

#include <stdio.h>
来源：http://qml.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://duk.andypj.xyz

[S02] C：变量与格式化输出
来源：http://eup.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://wzn.chenjidiqi.icu

[S03] C：读入整数
来源：http://jwh.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://mvn.yj20258.top

[S04] C：字符串复制
来源：http://nrt.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://rsg.xylfe.cn

[S05] C：字符串长度
来源：http://stq.sjlbkw.cn

strlen(s)
来源：http://tra.zhiwuduotai.top

[S06] C：字符串比较
来源：http://oiv.sxryk.cn

strcmp(a, b) == 0
来源：http://tat.hywenlv.cn

[S07] C：数组遍历求和
来源：http://ana.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mfo.hammf.cn

[S08] C：动态内存分配与释放
来源：http://viy.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qfk.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://mlp.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://awy.redwolf501.top

[S10] C：指针与解引用
来源：http://smi.bbcook.cn

int *p = &a;  *p = 5;
来源：http://qoe.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://hrq.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvq.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxx.nanxuanxn.top

fclose(f);
来源：http://xxg.sufxvd.cn

[S12] C：写文件
来源：http://alb.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tcr.quarkkingdee.top

[S13] C：宏定义
来源：http://zmq.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jzw.nwbrower.top

[S14] C：枚举
来源：http://qjr.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://dwl.jlsjyb.cn

[S15] C：类型转换
来源：http://fwv.jinqigufen.top

(double) a / b
来源：http://kgj.jqgufenzy.top

[S16] C：位操作置位
来源：http://nxf.sjlbkw.cn

x |= (1 << 3);
来源：http://fll.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://fbe.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hxp.jianghu66.top

[S18] C：命令行参数
来源：http://chp.nwbrower.top

int main(int argc, char **argv)
来源：http://jvm.gzhubu.top

[S19] C：快速排序
来源：http://xhe.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gdr.guowangkeji.top

[S20] C：二分查找
来源：http://lpf.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pcf.hnqzz.top

[S21] C：字符类别判断
来源：http://cvi.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ukp.yangfankeji.com

[S22] C：字符串转数字
来源：http://yai.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://nxg.52xcode.cn

[S23] C：随机数
来源：http://guu.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://viq.yj20258888.top

[S24] C：获取本地时间
来源：http://yez.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aft.ppjwa.cn

[S25] C：内存拷贝
来源：http://gym.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://akj.fengsongda.top

[S26] C：内存清零
来源：http://tua.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://act.yuanzhike.top

[S27] C：定义常量
来源：http://ryj.fzhhl.top

const double PI = 3.14159;
来源：http://jfl.fktsv.cn

[S28] C：静态变量
来源：http://mkb.yuxming.cn

static int counter = 0;
来源：http://evc.fanxiaobao.xyz

[S29] C：变参函数
来源：http://hgy.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ybs.epnwcf.com

[S30] C：头文件保护
来源：http://fmx.gotoacloud.top

#ifndef X_H
来源：http://cfi.jinqigfzy.top

#define X_H
来源：http://nhx.jlsjyb.cn

#endif
来源：http://kxs.yuanzhike.top

[S31] C++：Hello World
来源：http://rut.pengpengdd.cyou

#include <iostream>
来源：http://rcg.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://uef.ctjpmb.com

[S32] C++：字符串
来源：http://iwm.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://gdi.haohaochexian.top

[S33] C++：vector 增删
来源：http://xvo.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zdt.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://mpb.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://qaz.andypj.xyz

[S35] C++：map
来源：http://uqw.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ntn.aizwys.cn

[S36] C++：unordered_map
来源：http://exh.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fji.jinqigfzy.top

[S37] C++：set
来源：http://mbc.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pbi.jinyuanbaomall.cn

[S38] C++：排序
来源：http://lgl.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://sdw.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://joa.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxx.ydjk.org.cn

[S40] C++：查找元素
来源：http://pzp.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fxz.zdqjudy.top

[S41] C++：类与构造函数
来源：http://xgh.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xpi.xinyue.icu

[S42] C++：继承与虚函数
来源：http://drk.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://hgn.sjlbkw.cn

[S43] C++：智能指针
来源：http://kmm.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://dmk.hcnkem.com

[S44] C++：引用传参
来源：http://lwn.yj202588.top

void inc(int &x) { ++x; }
来源：http://fic.shzxlz.cn


<!-- 参考信息 -->