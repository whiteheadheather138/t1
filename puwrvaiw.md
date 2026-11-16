代发 wailian999

[Q67] 设置隔离级别
来源：http://ffg.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qwt.iojbl.cn

[Q68] 保存点
来源：http://lsn.hysaishi.cn

SAVEPOINT sp1;
来源：http://mka.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://usy.wangdashe.top

[Q69] 查看执行计划
来源：http://uwt.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nhd.hnxiangtu.top

[Q70] 更新统计信息
来源：http://dsa.tarul.cn

ANALYZE TABLE users;
来源：http://rdh.9152youxi.cn

[Q71] 查看建表语句
来源：http://cst.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qym.yueranfly.top

[Q72] 查看索引
来源：http://oif.hywenlv.cn

SHOW INDEX FROM users;
来源：http://tom.fktsv.cn

[Q73] 查看表状态
来源：http://cyv.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xjr.yuanzhike.top

[Q74] 强制使用索引
来源：http://nsc.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://smd.gotoacloud.top

[Q75] 日期格式化
来源：http://ezk.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ifc.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xyw.zdqjudy.top

[Q76] 按天统计
来源：http://vmm.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ptc.iojbl.cn

[Q77] 时间加减
来源：http://vna.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tgx.xinyue.icu

[Q78] 当前时间
来源：http://lyq.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://icp.cqqwz.cn

[Q79] 字符串拼接
来源：http://gcp.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fym.smart0.xyz

[Q80] 字符串截取
来源：http://yci.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://olq.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://vpc.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://soi.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://vjp.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aqn.ehwqpu.com

[Q83] 大小写转换
来源：http://sgs.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://spo.jqgfzy.top

[Q84] 去除首尾空格
来源：http://htp.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://mfn.cdnleiting.top

[Q85] 数值取整
来源：http://haq.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jqv.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://opy.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ugx.smart0.xyz

[Q87] JSON 字段做条件
来源：http://ztb.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rmm.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://pfn.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pga.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fov.jianghu66.top

[Q89] 判断表是否存在
来源：http://mbb.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://adu.yj202588.top

[Q90] 生成序号列
来源：http://kew.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zbi.yuanzhike.top

================================================================================
来源：http://guv.bjfxy.top

R. Bash 专题
来源：http://oap.0kj1m.cn

================================================================================
来源：http://cvu.chenzaomai.com

[R01] shebang 与严格模式
来源：http://dlu.ctjpmb.com

#!/usr/bin/env bash
来源：http://mjx.shuidangran.top

set -euo pipefail
来源：http://igf.0kj1m.cn

[R02] 变量赋值与使用
来源：http://mzh.zhengqikj.top

name="Tom"; echo "$name"
来源：http://fmi.mhx1999.top

[R03] 只读变量
来源：http://xyt.yj20258888.top

readonly PI=3.14
来源：http://wnh.yvedp.cn

[R04] 位置参数
来源：http://xoa.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rhd.sufxvd.cn

[R05] 参数默认值
来源：http://txc.shzxlz.cn

name="${1:-default}"
来源：http://esi.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://jcz.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xys.fktsv.cn

[R07] if 判断文件
来源：http://qrh.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fpb.xuetiantiany.cn

[R08] 数值比较
来源：http://mwm.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iyj.yonumen.top

[R09] 字符串比较
来源：http://mcw.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wbk.ctjpmb.com

[R10] 正则匹配
来源：http://xpr.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tun.meibo888.top

[R11] case 多分支
来源：http://pgi.zhoulong.xyz

case "$1" in
来源：http://ndp.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://sos.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://wpd.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://kxu.xinyue.icu

esac
来源：http://txe.wangshuangyany.cn

[R12] for 遍历文件
来源：http://mzc.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://sxr.pycfn.com

[R13] for 计数循环
来源：http://ubo.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://zsn.yuanzhike.top

[R14] C 风格 for
来源：http://ddk.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tyq.0kj1m.cn

[R15] while 逐行读文件
来源：http://tuv.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bpx.yj202588.top

[R16] until 等待条件
来源：http://due.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gwr.gotoacloud.top

[R17] 数组定义与取值
来源：http://wdu.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://utn.hcnkem.com

[R18] 遍历数组
来源：http://ohp.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bia.guannengcc.top

[R19] 数组长度
来源：http://qda.yuanzhike.top

echo "${#arr[@]}"
来源：http://bcq.hfpthk.cn

[R20] 关联数组（字典）
来源：http://pqx.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kbn.316326.xyz

[R21] 字符串长度
来源：http://mdq.zhoulong.xyz

echo "${#s}"
来源：http://asc.zdbjq.cn

[R22] 截取子串
来源：http://uvd.tianlin.xyz

echo "${s:0:5}"
来源：http://nge.chenjidiqi.icu

[R23] 字符串替换
来源：http://yjj.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ewb.xziqi.cn

[R24] 大小写转换
来源：http://zuz.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://lpv.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://jzn.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vmj.tarul.cn

[R26] 命令替换
来源：http://fvq.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://jsf.yj202588.top

[R27] 算术展开
来源：http://cra.mhx1999.top

echo $((1 + 2 * 3))
来源：http://hza.jqgfzy.top

[R28] 浮点运算
来源：http://kjl.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://pyw.fktsv.cn

[R29] 定义函数
来源：http://krq.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://flt.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://ovc.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://aec.snrcjt.cn

[R31] 局部变量
来源：http://its.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://mwa.hammf.cn

[R32] 参数个数校验
来源：http://gde.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hkx.hammf.cn

[R33] 捕获错误并提示行号
来源：http://cld.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hmg.jyoumei.cn

[R34] 退出时清理
来源：http://smd.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://twj.bbcook.cn

[R35] 后台执行并等待
来源：http://gst.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xhu.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://qen.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://low.sufxvd.cn

[R37] 把输出赋给变量
来源：http://bdv.hywenlv.cn

files=$(ls -1)
来源：http://cok.aibaodan.cn

[R38] 管道串联
来源：http://mtm.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://oru.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://zbf.pycfn.com

cmd > out.log 2>&1
来源：http://hrb.birdmap.top

[R40] 追加写日志
来源：http://hed.guannengcc.top

echo "log" >> out.log
来源：http://bei.hfpthk.cn

[R41] 丢弃输出
来源：http://zkh.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://tws.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://nju.fengsongda.top

wc -l < a.txt
来源：http://zkd.0kj1m.cn

[R43] 按名字查找文件
来源：http://til.ehwqpu.com

find . -name "*.log" -type f
来源：http://ucc.bbcook.cn

[R44] 按修改时间查找
来源：http://dhp.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://wzx.jiagoushi.top

[R45] 批量删除
来源：http://hdk.epnwcf.com

find . -name "*.tmp" -delete
来源：http://qpn.tarul.cn

[R46] 递归替换文件内容
来源：http://lnl.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lez.yuanzhike.top

[R47] sed 单行替换
来源：http://xoq.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://svp.cashguo.top

[R48] awk 取指定列
来源：http://pii.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://exk.daria6918.cn

[R49] awk 带条件
来源：http://kmo.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ati.xuanzx.com

[R50] awk 求和
来源：http://amh.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://qmq.smart0.xyz

[R51] 排序去重取前几
来源：http://iqr.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fbe.gaohongyu789.top

[R52] 统计行数
来源：http://vuk.chenzaomai.com

wc -l a.txt
来源：http://kco.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://ysr.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jae.jqgfzy.top

[R54] 比较两个文件
来源：http://uxy.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://jsv.xuanzx.com

[R55] 压缩与解压
来源：http://nqh.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zjf.tian-w.cn

[R56] 远程拷贝
来源：http://ypx.zhengqikj.top

scp file user@host:/path/
来源：http://ggl.wangdashe.top

[R57] 远程执行命令
来源：http://qcj.zhijiandao.cn

ssh user@host 'uptime'
来源：http://lgp.sweek.top

[R58] 下载文件
来源：http://xos.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://esm.gzhubu.top

[R59] 发 POST JSON
来源：http://ips.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zcl.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://esz.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fal.nanxinkj.top

[R61] 磁盘占用
来源：http://zxt.sysykeji.top

df -h;  du -sh *
来源：http://xlx.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://svz.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://mqz.hysaishi.cn

[R63] 内存与进程
来源：http://xes.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://oct.iojbl.cn

[R64] 结束进程
来源：http://tzp.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://hpf.bjfxy.top

[R65] 查看端口占用
来源：http://dsl.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eej.ybcxt.top

[R66] 定时任务
来源：http://one.yangfankeji.com

crontab -e;  crontab -l
来源：http://cir.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://akt.c1oappe.top

openssl rand -hex 16
来源：http://dgc.haohaochexian.top

[R68] 计算文件校验值
来源：http://txa.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://nsq.mhx1999.top

[R69] 生成随机密码
来源：http://zmo.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://dsg.0kj1m.cn

[R70] 时间戳与互转
来源：http://jfl.wangdashe.top

date +%s;  date -d @1700000000
来源：http://msi.jinghuilouyu.cn

[R71] 日期格式化
来源：http://vzy.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://anh.cucudq.cn

[R72] 等待端口就绪
来源：http://taj.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://lvc.hfpthk.cn

[R73] 分割大日志
来源：http://sjc.c1oappe.top

split -l 1000 big.log part_
来源：http://ssy.jianghu66.top

[R74] 批量重命名
来源：http://xqw.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://knh.zycfv.cn

[R75] 导出环境变量
来源：http://kkz.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://eox.xuetiantiany.cn

[R76] 使用临时文件
来源：http://zsw.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zds.vehdjk.com

[R77] 读取用户输入
来源：http://zuy.smart0.xyz

read -rp "请输入: " ans
来源：http://fqi.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://fdi.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dkx.aizwys.cn

[R79] 解析命令行选项
来源：http://oxf.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sdk.tarul.cn

[R80] 查看脚本执行耗时
来源：http://kyl.52xcode.cn

time ./run.sh
来源：http://cog.xziqi.cn

================================================================================
来源：http://xoi.zhoulong.xyz

S. C / C++ 专题
来源：http://usy.fanxiaobao.xyz

================================================================================
来源：http://vtw.yuanzhike.top

[S01] C：Hello World
来源：http://emk.jianghu66.top

#include <stdio.h>
来源：http://vlb.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jvn.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://krh.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://xah.yj202588.top

[S03] C：读入整数
来源：http://ecc.iojbl.cn

int x; scanf("%d", &x);
来源：http://bmd.hnqzz.top

[S04] C：字符串复制
来源：http://rav.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://tdf.tian-w.cn

[S05] C：字符串长度
来源：http://zom.jianghu66.top

strlen(s)
来源：http://afa.shzxlz.cn

[S06] C：字符串比较
来源：http://ugl.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://tqs.chenzaomai.com

[S07] C：数组遍历求和
来源：http://efi.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cwu.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://tjc.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zyo.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://pwb.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dib.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://ddu.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://ohp.yuxming.cn

[S11] C：逐行读文件
来源：http://xcf.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://ila.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hqo.zhoulong.xyz

fclose(f);
来源：http://mms.smart0.xyz

[S12] C：写文件
来源：http://pzg.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pjg.fktsv.cn

[S13] C：宏定义
来源：http://vhv.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yfl.ivvv.top

[S14] C：枚举
来源：http://cun.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://nrf.tian-w.cn

[S15] C：类型转换
来源：http://lrg.ydzc1.top

(double) a / b
来源：http://umd.tian-w.cn

[S16] C：位操作置位
来源：http://xia.hnxiangtu.top

x |= (1 << 3);
来源：http://vgu.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://enl.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syf.uphjek.com

[S18] C：命令行参数
来源：http://mvo.cqqwz.cn

int main(int argc, char **argv)
来源：http://lvf.zhengqikj.top

[S19] C：快速排序
来源：http://gau.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://lxl.jyoumei.cn

[S20] C：二分查找
来源：http://cev.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gcj.hammf.cn

[S21] C：字符类别判断
来源：http://rdd.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://puj.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://dxh.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bdu.gaohongyu789.top

[S23] C：随机数
来源：http://mbp.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://svq.gzhubu.top

[S24] C：获取本地时间
来源：http://zke.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bae.cdnleiting.top

[S25] C：内存拷贝
来源：http://clv.316326.xyz

memcpy(dst, src, n);
来源：http://jap.hesvh.cn

[S26] C：内存清零
来源：http://ywq.yuxming.cn

memset(a, 0, sizeof a);
来源：http://spm.yj202588.top

[S27] C：定义常量
来源：http://msm.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://gwz.iojbl.cn

[S28] C：静态变量
来源：http://eue.smart0.xyz

static int counter = 0;
来源：http://uyd.zycfv.cn

[S29] C：变参函数
来源：http://cpf.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vri.ybcxt.top

[S30] C：头文件保护
来源：http://jgb.hfpthk.cn

#ifndef X_H
来源：http://gyg.shuidangran.top

#define X_H
来源：http://rfy.sysykeji.top

#endif
来源：http://eip.yueranfly.top

[S31] C++：Hello World
来源：http://sai.shangyingyoupin.top

#include <iostream>
来源：http://ukt.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://vys.chenzaomai.com

[S32] C++：字符串
来源：http://yxo.pycfn.com

std::string s = "hi";  s += "!";
来源：http://jqr.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://jxn.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mpk.c1oappe.top

[S34] C++：遍历 vector
来源：http://qdl.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://mla.yuanzhike.top

[S35] C++：map
来源：http://jux.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hyn.quarkkingdee.top

[S36] C++：unordered_map
来源：http://gtq.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gqk.daxiang520.top


<!-- 参考信息 -->