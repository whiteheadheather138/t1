代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wsh.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://uay.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gdj.havefunace.top

[Q57] 行号
来源：http://ikm.ivvv.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tdt.chenzaomai.com

[Q58] 累计求和
来源：http://ocb.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xyv.feifeiyinyue.top

[Q59] 分组内累计
来源：http://rwa.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dwk.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://bjf.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gtt.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nix.svipenyu.cn

[Q61] 移动平均
来源：http://sml.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cbl.jianghu66.top

[Q62] 分组占比
来源：http://tqp.yueranfly.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rta.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://mxs.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zmv.hammf.cn

[Q64] 提交事务
来源：http://qlp.yj20258.top

COMMIT;
来源：http://mcr.shzxlz.cn

[Q65] 回滚事务
来源：http://uvn.cucudq.cn

ROLLBACK;
来源：http://hbe.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://dqk.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hcr.andypj.xyz

[Q67] 设置隔离级别
来源：http://hda.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eyh.meibo888.top

[Q68] 保存点
来源：http://ylu.fzhhl.top

SAVEPOINT sp1;
来源：http://rtq.hysaishi.cn

ROLLBACK TO sp1;
来源：http://scv.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://ueb.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kzv.9152youxi.cn

[Q70] 更新统计信息
来源：http://yje.tanke756.top

ANALYZE TABLE users;
来源：http://hut.wangdashe.top

[Q71] 查看建表语句
来源：http://kai.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xqq.fanxiaobao.xyz

[Q72] 查看索引
来源：http://mgz.fehbvm.com

SHOW INDEX FROM users;
来源：http://onu.ydjk.org.cn

[Q73] 查看表状态
来源：http://clm.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wtk.sysykeji.top

[Q74] 强制使用索引
来源：http://ask.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cxi.nanxinkj.top

[Q75] 日期格式化
来源：http://gcy.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mbk.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nrc.feifeiyinyue.top

[Q76] 按天统计
来源：http://sef.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kuk.jiagoushi.top

[Q77] 时间加减
来源：http://jgc.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fjh.quarkkingdee.top

[Q78] 当前时间
来源：http://wre.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uwx.xziqi.cn

[Q79] 字符串拼接
来源：http://jph.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xgo.shangyingyoupin.top

[Q80] 字符串截取
来源：http://kan.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vnn.jinqigfzy.top

[Q81] 字符串替换
来源：http://zze.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cff.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://qjm.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lll.yueranfly.top

[Q83] 大小写转换
来源：http://gfp.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kgv.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://nsi.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://rzm.jiagoushi.top

[Q85] 数值取整
来源：http://ile.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mbo.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://qkw.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://owo.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://ite.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fth.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://qtd.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://war.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uqc.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://pxu.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://drl.zhoulong.xyz

[Q90] 生成序号列
来源：http://ltn.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dsn.kuanghao11.cn

================================================================================
来源：http://twv.nwbrower.top

R. Bash 专题
来源：http://hqc.pengpengdd.cyou

================================================================================
来源：http://muw.daria6918.cn

[R01] shebang 与严格模式
来源：http://xki.guannengcc.top

#!/usr/bin/env bash
来源：http://ssz.ehwqpu.com

set -euo pipefail
来源：http://waa.hesvh.cn

[R02] 变量赋值与使用
来源：http://svd.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://meo.hcnkem.com

[R03] 只读变量
来源：http://stf.xuetiantiany.cn

readonly PI=3.14
来源：http://rnc.jinyuanbaomall.cn

[R04] 位置参数
来源：http://zhy.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zij.daria6918.cn

[R05] 参数默认值
来源：http://krm.zhengqikj.top

name="${1:-default}"
来源：http://its.0kj1m.cn

[R06] 判断命令是否存在
来源：http://unr.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wal.hongshengwenyu.top

[R07] if 判断文件
来源：http://bmj.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nwf.hnqzz.top

[R08] 数值比较
来源：http://qnu.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://idi.cqqwz.cn

[R09] 字符串比较
来源：http://juj.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ddb.nanxinkj.top

[R10] 正则匹配
来源：http://jsp.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lke.xuetiantiany.cn

[R11] case 多分支
来源：http://lsq.cqqwz.cn

case "$1" in
来源：http://eil.yonumen.top

start) echo "启动" ;;
来源：http://xqc.andypj.xyz

stop)  echo "停止" ;;
来源：http://hzc.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://zlz.ivvv.top

esac
来源：http://gcd.yanxiufei.cn

[R12] for 遍历文件
来源：http://jzp.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://grj.hywenlv.cn

[R13] for 计数循环
来源：http://psf.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://jkc.epnwcf.com

[R14] C 风格 for
来源：http://hod.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lsb.xuanzx.com

[R15] while 逐行读文件
来源：http://abf.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hcq.ehwqpu.com

[R16] until 等待条件
来源：http://cky.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bsb.dashuyun.cn

[R17] 数组定义与取值
来源：http://rsv.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://ieo.zhoulong.xyz

[R18] 遍历数组
来源：http://mai.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cng.yfazqb.com

[R19] 数组长度
来源：http://uzg.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://cim.bbcook.cn

[R20] 关联数组（字典）
来源：http://rot.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svk.aibaodan.cn

[R21] 字符串长度
来源：http://yti.hcnkem.com

echo "${#s}"
来源：http://jhx.svipenyu.cn

[R22] 截取子串
来源：http://lhu.guannengcc.top

echo "${s:0:5}"
来源：http://fnt.xylfe.cn

[R23] 字符串替换
来源：http://dhw.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pkd.ybcxt.top

[R24] 大小写转换
来源：http://ejd.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dej.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://wgu.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bdf.jlsjyb.cn

[R26] 命令替换
来源：http://ccx.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://xjj.zhijiandao.cn

[R27] 算术展开
来源：http://fvp.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://iiy.andypj.xyz

[R28] 浮点运算
来源：http://qhk.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://zkz.zhixingplan.top

[R29] 定义函数
来源：http://lje.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tbd.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://bcq.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://rnt.gotoacloud.top

[R31] 局部变量
来源：http://nwb.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://cdq.yangfankeji.com

[R32] 参数个数校验
来源：http://spm.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jpq.tanke756.top

[R33] 捕获错误并提示行号
来源：http://rdr.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hdg.52xcode.cn

[R34] 退出时清理
来源：http://eop.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://muy.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://cjm.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pby.cashguo.top

[R36] 并发执行多个任务
来源：http://mmp.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hvh.hnqzz.top

[R37] 把输出赋给变量
来源：http://pyn.ivvv.top

files=$(ls -1)
来源：http://hlp.ydjk.org.cn

[R38] 管道串联
来源：http://axb.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://ohy.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://pdf.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://lcr.hnqzz.top

[R40] 追加写日志
来源：http://cyf.hfpthk.cn

echo "log" >> out.log
来源：http://krl.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://uka.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://hhh.hongshengwenyu.top

[R42] 输入重定向
来源：http://ndr.sweek.top

wc -l < a.txt
来源：http://qcv.aizwys.cn

[R43] 按名字查找文件
来源：http://tmf.daria6918.cn

find . -name "*.log" -type f
来源：http://min.tian-w.cn

[R44] 按修改时间查找
来源：http://bhf.yj20258.top

find . -mtime -7 -type f
来源：http://pcw.sjlbkw.cn

[R45] 批量删除
来源：http://deo.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://fwy.c1oappe.top

[R46] 递归替换文件内容
来源：http://rhn.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gim.jiagoushi.top

[R47] sed 单行替换
来源：http://fcv.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://kwu.aibaodan.cn

[R48] awk 取指定列
来源：http://vhm.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://orn.hcnkem.com

[R49] awk 带条件
来源：http://qap.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qll.hammf.cn

[R50] awk 求和
来源：http://oht.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://jtk.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://btc.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yva.ydjk.org.cn

[R52] 统计行数
来源：http://pya.andypj.xyz

wc -l a.txt
来源：http://jon.tarul.cn

[R53] 查看文件头与实时尾
来源：http://fhe.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xpu.guowangkeji.top

[R54] 比较两个文件
来源：http://dap.nanxuanxn.top

diff a.txt b.txt
来源：http://kvs.xuanzx.com

[R55] 压缩与解压
来源：http://kyo.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ent.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://sov.ydjk.org.cn

scp file user@host:/path/
来源：http://fqb.haohaochexian.top

[R57] 远程执行命令
来源：http://ssp.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://dhm.0kj1m.cn

[R58] 下载文件
来源：http://ivc.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uaq.uphjek.com

[R59] 发 POST JSON
来源：http://frl.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://maw.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://cfc.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fom.zhixingplan.top

[R61] 磁盘占用
来源：http://jli.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://iei.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://usj.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://fha.jinghuilouyu.cn

[R63] 内存与进程
来源：http://mfi.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://ghv.quarkkingdee.top

[R64] 结束进程
来源：http://ckt.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://oge.shangyingyoupin.top

[R65] 查看端口占用
来源：http://mnu.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ccy.daxiang520.top

[R66] 定时任务
来源：http://hmf.hnqzz.top

crontab -e;  crontab -l
来源：http://nfg.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://tzs.zdbjq.cn

openssl rand -hex 16
来源：http://oky.kuanghao11.cn

[R68] 计算文件校验值
来源：http://wxv.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://rhk.smart0.xyz

[R69] 生成随机密码
来源：http://rxm.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://mis.jianghu66.top

[R70] 时间戳与互转
来源：http://nml.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://uef.svipenyu.cn

[R71] 日期格式化
来源：http://zkm.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://omj.fengsongda.top

[R72] 等待端口就绪
来源：http://ian.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://srf.yj20258.top

[R73] 分割大日志
来源：http://ngs.nanxuanxn.top

split -l 1000 big.log part_
来源：http://idd.hfpthk.cn

[R74] 批量重命名
来源：http://bjt.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qfc.aizwys.cn

[R75] 导出环境变量
来源：http://ffe.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://rte.jinqigfzy.top

[R76] 使用临时文件
来源：http://bnv.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ulz.fzhhl.top

[R77] 读取用户输入
来源：http://gmj.kuanghao11.cn

read -rp "请输入: " ans
来源：http://veo.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://xfg.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eug.xylfe.cn

[R79] 解析命令行选项
来源：http://hvo.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://toa.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://uyf.chenlongwang.top

time ./run.sh
来源：http://uqh.snrcjt.cn

================================================================================
来源：http://pck.zdbjq.cn

S. C / C++ 专题
来源：http://wtp.shuidangran.top

================================================================================
来源：http://kyr.jianghu66.top

[S01] C：Hello World
来源：http://oij.ydjk.org.cn

#include <stdio.h>
来源：http://avv.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://att.xziqi.cn

[S02] C：变量与格式化输出
来源：http://gfw.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://epc.cashguo.top

[S03] C：读入整数
来源：http://tav.vehdjk.com

int x; scanf("%d", &x);
来源：http://wft.gzhubu.top

[S04] C：字符串复制
来源：http://dte.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://byc.sysykeji.top

[S05] C：字符串长度
来源：http://cau.xziqi.cn

strlen(s)
来源：http://zip.hongshengwenyu.top

[S06] C：字符串比较
来源：http://bgh.haohaochexian.top

strcmp(a, b) == 0
来源：http://jpv.xziqi.cn

[S07] C：数组遍历求和
来源：http://nap.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ncu.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://xux.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kff.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://qmm.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tek.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://nvl.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://ejx.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://veb.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://kjp.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fat.uphjek.com

fclose(f);
来源：http://rhd.zycfv.cn

[S12] C：写文件
来源：http://pcd.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gqh.yongpay.top

[S13] C：宏定义
来源：http://kis.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ads.ywan-chungtsiang.top

[S14] C：枚举
来源：http://hdk.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://lnk.hcnkem.com

[S15] C：类型转换
来源：http://tcb.ybcxt.top

(double) a / b
来源：http://umu.zhoulong.xyz

[S16] C：位操作置位
来源：http://fcr.hywenlv.cn

x |= (1 << 3);
来源：http://buu.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://maj.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ckn.jlsjyb.cn

[S18] C：命令行参数
来源：http://bfj.guowangkeji.top

int main(int argc, char **argv)
来源：http://hig.jinghuilouyu.cn

[S19] C：快速排序
来源：http://btf.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bal.xylfe.cn

[S20] C：二分查找
来源：http://mnn.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fyo.andypj.xyz

[S21] C：字符类别判断
来源：http://bnh.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://egk.mhx1999.top

[S22] C：字符串转数字
来源：http://vvl.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fbw.jqgufenzy.top

[S23] C：随机数
来源：http://gfp.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ton.tarul.cn

[S24] C：获取本地时间
来源：http://yep.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qkp.daxiang520.top

[S25] C：内存拷贝
来源：http://cnm.ydzc1.top

memcpy(dst, src, n);
来源：http://sis.yangfankeji.com

[S26] C：内存清零
来源：http://dbv.tian-w.cn


<!-- 参考信息 -->