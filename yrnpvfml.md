代发 wailian999

[Q63] 开启事务
来源：http://ypv.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vlm.ivvv.top

[Q64] 提交事务
来源：http://stx.cheryme.top

COMMIT;
来源：http://bgs.shzxlz.cn

[Q65] 回滚事务
来源：http://vkh.guannengcc.top

ROLLBACK;
来源：http://yxa.xylfe.cn

[Q66] 行锁查询
来源：http://skz.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hjd.yongpay.top

[Q67] 设置隔离级别
来源：http://xmh.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tlt.ywan-chungtsiang.top

[Q68] 保存点
来源：http://rtp.cheryme.top

SAVEPOINT sp1;
来源：http://ejw.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://kge.tianlin.xyz

[Q69] 查看执行计划
来源：http://kav.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dgb.yanxiufei.cn

[Q70] 更新统计信息
来源：http://lww.hfpthk.cn

ANALYZE TABLE users;
来源：http://sac.yuxming.cn

[Q71] 查看建表语句
来源：http://uiy.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zji.wangshuangyany.cn

[Q72] 查看索引
来源：http://sqp.hnqzz.top

SHOW INDEX FROM users;
来源：http://isa.9152youxi.cn

[Q73] 查看表状态
来源：http://azt.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lug.yfazqb.com

[Q74] 强制使用索引
来源：http://yed.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lwr.aizwys.cn

[Q75] 日期格式化
来源：http://jyf.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xqo.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ldt.yvedp.cn

[Q76] 按天统计
来源：http://qnl.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ttc.meibo888.top

[Q77] 时间加减
来源：http://jfo.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dye.svipenyu.cn

[Q78] 当前时间
来源：http://lab.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qhc.yanxiufei.cn

[Q79] 字符串拼接
来源：http://tob.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bsb.smart0.xyz

[Q80] 字符串截取
来源：http://jks.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dsp.zhoulong.xyz

[Q81] 字符串替换
来源：http://itn.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ips.yj202588.top

[Q82] 字符长度与字节长度
来源：http://aoh.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://seo.shzxlz.cn

[Q83] 大小写转换
来源：http://dij.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sbl.aibaodan.cn

[Q84] 去除首尾空格
来源：http://bsk.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://eja.52xcode.cn

[Q85] 数值取整
来源：http://hco.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eqi.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://wsq.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dao.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://bkj.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wpi.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://kin.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://auf.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hig.xziqi.cn

[Q89] 判断表是否存在
来源：http://ddb.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ktd.zhengqikj.top

[Q90] 生成序号列
来源：http://jcp.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kut.jinyuanbaomall.cn

================================================================================
来源：http://xul.xuetiantiany.cn

R. Bash 专题
来源：http://ccs.ybcxt.top

================================================================================
来源：http://lse.haohaochexian.top

[R01] shebang 与严格模式
来源：http://ota.xziqi.cn

#!/usr/bin/env bash
来源：http://fww.uphjek.com

set -euo pipefail
来源：http://llw.52xcode.cn

[R02] 变量赋值与使用
来源：http://ben.yj20258888.top

name="Tom"; echo "$name"
来源：http://yjp.fzhhl.top

[R03] 只读变量
来源：http://kjs.cheryme.top

readonly PI=3.14
来源：http://too.bjfxy.top

[R04] 位置参数
来源：http://prv.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://txj.daxiang520.top

[R05] 参数默认值
来源：http://cqj.gaohongyu789.top

name="${1:-default}"
来源：http://luf.havefunace.top

[R06] 判断命令是否存在
来源：http://ywx.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://njs.jyoumei.cn

[R07] if 判断文件
来源：http://ngr.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zsu.dianchejie.cn

[R08] 数值比较
来源：http://cef.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aun.sufxvd.cn

[R09] 字符串比较
来源：http://mjc.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lmq.meibo888.top

[R10] 正则匹配
来源：http://yeo.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ldj.xuanzx.com

[R11] case 多分支
来源：http://fug.fanxiaobao.xyz

case "$1" in
来源：http://hfc.daxiang520.top

start) echo "启动" ;;
来源：http://hkc.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://ccs.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://crw.bbcook.cn

esac
来源：http://mbu.fktsv.cn

[R12] for 遍历文件
来源：http://cdl.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://yye.yuxming.cn

[R13] for 计数循环
来源：http://ylr.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://pim.redwolf501.top

[R14] C 风格 for
来源：http://zem.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://edl.yuxming.cn

[R15] while 逐行读文件
来源：http://mmd.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nmz.9152youxi.cn

[R16] until 等待条件
来源：http://ega.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mdv.chenlongwang.top

[R17] 数组定义与取值
来源：http://ieu.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wjm.zdqjudy.top

[R18] 遍历数组
来源：http://wsq.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wbh.gaohongyu789.top

[R19] 数组长度
来源：http://icq.0kj1m.cn

echo "${#arr[@]}"
来源：http://pco.zhengqikj.top

[R20] 关联数组（字典）
来源：http://sdp.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sob.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://ylf.dianchejie.cn

echo "${#s}"
来源：http://ahg.yj20258888.top

[R22] 截取子串
来源：http://xgr.zdbjq.cn

echo "${s:0:5}"
来源：http://oaw.smart0.xyz

[R23] 字符串替换
来源：http://mig.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bfl.chenjidiqi.icu

[R24] 大小写转换
来源：http://tqw.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nzl.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://mik.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://prc.gzhubu.top

[R26] 命令替换
来源：http://jhe.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://sof.xinyue.icu

[R27] 算术展开
来源：http://fmz.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://swk.cashguo.top

[R28] 浮点运算
来源：http://uyy.sweek.top

echo "scale=2; 10/3" | bc
来源：http://pkq.shanyushiyangtech.top

[R29] 定义函数
来源：http://zgc.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://plv.andypj.xyz

[R30] 函数返回状态码
来源：http://rsy.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://kkk.ydzc1.top

[R31] 局部变量
来源：http://nwk.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://ohe.yuxming.cn

[R32] 参数个数校验
来源：http://zkh.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qwk.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://pzc.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://enk.0kj1m.cn

[R34] 退出时清理
来源：http://vbq.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://uaz.birdmap.top

[R35] 后台执行并等待
来源：http://fki.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ihc.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://hbo.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qev.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://evv.hnxiangtu.top

files=$(ls -1)
来源：http://eam.jqgfzy.top

[R38] 管道串联
来源：http://sgu.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://gkd.tarul.cn

[R39] 重定向标准输出与错误
来源：http://mxw.hnqzz.top

cmd > out.log 2>&1
来源：http://ntl.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://nyd.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://tdb.ybcxt.top

[R41] 丢弃输出
来源：http://imo.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://zdg.zhiwuduotai.top

[R42] 输入重定向
来源：http://rfz.gotoacloud.top

wc -l < a.txt
来源：http://juw.zhijiandao.cn

[R43] 按名字查找文件
来源：http://dxg.bbcook.cn

find . -name "*.log" -type f
来源：http://jwp.ybcxt.top

[R44] 按修改时间查找
来源：http://tkk.yj20258888.top

find . -mtime -7 -type f
来源：http://uii.cqqwz.cn

[R45] 批量删除
来源：http://vwg.ybcxt.top

find . -name "*.tmp" -delete
来源：http://iwz.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://fpb.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kdk.zhengqikj.top

[R47] sed 单行替换
来源：http://kug.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://lfc.meibo888.top

[R48] awk 取指定列
来源：http://luk.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://hag.hongshengwenyu.top

[R49] awk 带条件
来源：http://ipt.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bsw.zhiwuduotai.top

[R50] awk 求和
来源：http://tdc.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://xdm.yonumen.top

[R51] 排序去重取前几
来源：http://oag.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hiv.shuidangran.top

[R52] 统计行数
来源：http://jxz.chenzaomai.com

wc -l a.txt
来源：http://fbw.zhijiandao.cn

[R53] 查看文件头与实时尾
来源：http://uob.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://flg.quarkkingdee.top

[R54] 比较两个文件
来源：http://vze.yuanzhike.top

diff a.txt b.txt
来源：http://mrm.c1oappe.top

[R55] 压缩与解压
来源：http://ehi.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qjp.chenlongwang.top

[R56] 远程拷贝
来源：http://wpy.jyoumei.cn

scp file user@host:/path/
来源：http://lyg.shzxlz.cn

[R57] 远程执行命令
来源：http://mmm.hnxiangtu.top

ssh user@host 'uptime'
来源：http://tpu.hnxiangtu.top

[R58] 下载文件
来源：http://txq.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ttc.zhongyouzk.top

[R59] 发 POST JSON
来源：http://htt.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ali.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://vzq.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kvy.bbcook.cn

[R61] 磁盘占用
来源：http://vkf.zdbjq.cn

df -h;  du -sh *
来源：http://jum.andypj.xyz

[R62] 找最占空间的文件
来源：http://vly.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://ccz.gaohongyu789.top

[R63] 内存与进程
来源：http://mvu.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://ftv.jyoumei.cn

[R64] 结束进程
来源：http://etc.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://gzg.52xcode.cn

[R65] 查看端口占用
来源：http://hrl.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gpi.feifeiyinyue.top

[R66] 定时任务
来源：http://kjz.chenzaomai.com

crontab -e;  crontab -l
来源：http://pzw.hnqzz.top

[R67] 生成随机十六进制串
来源：http://ddk.zdqjudy.top

openssl rand -hex 16
来源：http://foo.9152youxi.cn

[R68] 计算文件校验值
来源：http://xtg.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://fwu.nanxuanxn.top

[R69] 生成随机密码
来源：http://ymf.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://qav.kuanghao11.cn

[R70] 时间戳与互转
来源：http://htf.fengsongda.top

date +%s;  date -d @1700000000
来源：http://idk.aibaodan.cn

[R71] 日期格式化
来源：http://azy.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dxh.cqqwz.cn

[R72] 等待端口就绪
来源：http://ctl.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cms.uphjek.com

[R73] 分割大日志
来源：http://ner.epnwcf.com

split -l 1000 big.log part_
来源：http://xpq.ehwqpu.com

[R74] 批量重命名
来源：http://xhl.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tdu.sjlbkw.cn

[R75] 导出环境变量
来源：http://icx.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://kjh.bjfxy.top

[R76] 使用临时文件
来源：http://npm.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dze.c1oappe.top

[R77] 读取用户输入
来源：http://zek.kuanghao11.cn

read -rp "请输入: " ans
来源：http://cgk.havefunace.top

[R78] 交互式菜单
来源：http://yem.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lml.shzxlz.cn

[R79] 解析命令行选项
来源：http://ftj.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iwb.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://kgj.xuanzx.com

time ./run.sh
来源：http://tdv.sysykeji.top

================================================================================
来源：http://mwv.havefunace.top

S. C / C++ 专题
来源：http://lui.tarul.cn

================================================================================
来源：http://cob.hesvh.cn

[S01] C：Hello World
来源：http://tep.tian-w.cn

#include <stdio.h>
来源：http://nno.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dbd.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://nlz.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://glw.c1oappe.top

[S03] C：读入整数
来源：http://xsj.ctjpmb.com

int x; scanf("%d", &x);
来源：http://esy.yanxiufei.cn

[S04] C：字符串复制
来源：http://ahc.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://iqk.sxryk.cn

[S05] C：字符串长度
来源：http://srl.bjfxy.top

strlen(s)
来源：http://dro.ybcxt.top

[S06] C：字符串比较
来源：http://oui.hywenlv.cn

strcmp(a, b) == 0
来源：http://dma.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://jta.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vug.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://gsj.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pry.birdmap.top

[S09] C：结构体定义与初始化
来源：http://orb.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ymy.meibo888.top

[S10] C：指针与解引用
来源：http://aty.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://knf.vehdjk.com

[S11] C：逐行读文件
来源：http://ssz.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://bme.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kis.gogol.net.cn

fclose(f);
来源：http://nzq.jianghu66.top

[S12] C：写文件
来源：http://weu.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xew.zhoulong.xyz

[S13] C：宏定义
来源：http://rhh.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sjb.zycfv.cn

[S14] C：枚举
来源：http://gxr.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://ttf.ybcxt.top

[S15] C：类型转换
来源：http://tkn.aibaodan.cn

(double) a / b
来源：http://cyw.hysaishi.cn

[S16] C：位操作置位
来源：http://veb.yonumen.top

x |= (1 << 3);
来源：http://dqq.sweek.top

[S17] C：安全拼接字符串
来源：http://uxk.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qmq.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://foz.vqdsnc.cn

int main(int argc, char **argv)
来源：http://rci.fanxiaobao.xyz

[S19] C：快速排序
来源：http://jxw.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://eqc.hysaishi.cn

[S20] C：二分查找
来源：http://fzg.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vnr.zdbjq.cn

[S21] C：字符类别判断
来源：http://vna.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bhf.yj20258.top

[S22] C：字符串转数字
来源：http://mth.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://yzs.haohaochexian.top

[S23] C：随机数
来源：http://dyi.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fpr.tarul.cn

[S24] C：获取本地时间
来源：http://jhg.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://exl.hammf.cn

[S25] C：内存拷贝
来源：http://ywm.guowangkeji.top

memcpy(dst, src, n);
来源：http://ams.tianlin.xyz

[S26] C：内存清零
来源：http://atb.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://hjk.ehwqpu.com

[S27] C：定义常量
来源：http://sup.zhengqikj.top

const double PI = 3.14159;
来源：http://jgq.sweek.top

[S28] C：静态变量
来源：http://ter.ydjk.org.cn

static int counter = 0;
来源：http://aqs.vqdsnc.cn

[S29] C：变参函数
来源：http://qmv.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bou.xziqi.cn

[S30] C：头文件保护
来源：http://zle.zhoulong.xyz

#ifndef X_H
来源：http://qpx.yueranfly.top

#define X_H
来源：http://mit.yj202588.top

#endif
来源：http://sok.tarul.cn

[S31] C++：Hello World
来源：http://jqg.guowangkeji.top

#include <iostream>
来源：http://auv.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://vdh.dianchejie.cn

[S32] C++：字符串
来源：http://vmv.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://ulw.xingfuxueyuan.xyz


<!-- 参考信息 -->