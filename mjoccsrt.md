代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fvc.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://dae.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zvz.havefunace.top

[Q57] 行号
来源：http://hrj.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lzc.zdqjudy.top

[Q58] 累计求和
来源：http://nbp.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gah.guannengcc.top

[Q59] 分组内累计
来源：http://lwh.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fvx.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://qtc.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tfx.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zzy.jinqigufen.top

[Q61] 移动平均
来源：http://exs.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://snu.zhongyouzk.top

[Q62] 分组占比
来源：http://vff.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kvf.fktsv.cn

[Q63] 开启事务
来源：http://kqx.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fil.bbcook.cn

[Q64] 提交事务
来源：http://bpz.zhiwuduotai.top

COMMIT;
来源：http://jnd.nanxinkj.top

[Q65] 回滚事务
来源：http://aob.vehdjk.com

ROLLBACK;
来源：http://uxz.hfpthk.cn

[Q66] 行锁查询
来源：http://fde.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hhd.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://gai.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bkj.jqgufenzy.top

[Q68] 保存点
来源：http://cid.guowangkeji.top

SAVEPOINT sp1;
来源：http://ihz.tian-w.cn

ROLLBACK TO sp1;
来源：http://fuu.yanxiufei.cn

[Q69] 查看执行计划
来源：http://sil.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pmp.hnqzz.top

[Q70] 更新统计信息
来源：http://gpe.jqgufenzy.top

ANALYZE TABLE users;
来源：http://gpa.jianghu66.top

[Q71] 查看建表语句
来源：http://vve.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ogk.yj202588.top

[Q72] 查看索引
来源：http://syi.cucudq.cn

SHOW INDEX FROM users;
来源：http://ugw.mhx1999.top

[Q73] 查看表状态
来源：http://shk.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zko.yonumen.top

[Q74] 强制使用索引
来源：http://xrw.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qwy.birdmap.top

[Q75] 日期格式化
来源：http://vrv.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ryr.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hfi.havefunace.top

[Q76] 按天统计
来源：http://aau.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://peo.yueranfly.top

[Q77] 时间加减
来源：http://ojs.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://syi.aizwys.cn

[Q78] 当前时间
来源：http://yqf.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mlg.yj20258.top

[Q79] 字符串拼接
来源：http://izz.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jfy.sjlbkw.cn

[Q80] 字符串截取
来源：http://kvw.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dsf.pycfn.com

[Q81] 字符串替换
来源：http://bra.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://usr.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://rlk.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rxl.pengpengdd.cyou

[Q83] 大小写转换
来源：http://tdh.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://efw.sufxvd.cn

[Q84] 去除首尾空格
来源：http://ooy.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://fdq.wangdashe.top

[Q85] 数值取整
来源：http://xeq.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://one.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://znf.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://txz.yj20258.top

[Q87] JSON 字段做条件
来源：http://ndw.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://imr.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://gbx.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xef.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nxq.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://zip.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lfg.fzhhl.top

[Q90] 生成序号列
来源：http://thj.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ikl.yvedp.cn

================================================================================
来源：http://agp.ybcxt.top

R. Bash 专题
来源：http://epu.jqgfzy.top

================================================================================
来源：http://tnz.316326.xyz

[R01] shebang 与严格模式
来源：http://ilc.yj20258.top

#!/usr/bin/env bash
来源：http://avi.zdbjq.cn

set -euo pipefail
来源：http://qvn.zycfv.cn

[R02] 变量赋值与使用
来源：http://jla.cqqwz.cn

name="Tom"; echo "$name"
来源：http://szq.nanxuanxn.top

[R03] 只读变量
来源：http://jia.pengpengdd.cyou

readonly PI=3.14
来源：http://uby.daria6918.cn

[R04] 位置参数
来源：http://pgw.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uqn.dianchejie.cn

[R05] 参数默认值
来源：http://mbf.hammf.cn

name="${1:-default}"
来源：http://sdw.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://rsb.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rnz.yongpay.top

[R07] if 判断文件
来源：http://mbk.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dlg.jiagoushi.top

[R08] 数值比较
来源：http://qxr.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://onv.feifeiyinyue.top

[R09] 字符串比较
来源：http://xmp.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fpa.svipenyu.cn

[R10] 正则匹配
来源：http://cpd.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nrz.yongpay.top

[R11] case 多分支
来源：http://qnj.c1oappe.top

case "$1" in
来源：http://mwb.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://xjw.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://tsa.ybcxt.top

*)     echo "未知命令" ;;
来源：http://hur.sjlbkw.cn

esac
来源：http://ujz.mhx1999.top

[R12] for 遍历文件
来源：http://cvr.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://sst.ybcxt.top

[R13] for 计数循环
来源：http://dmo.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qpa.nanxuanxn.top

[R14] C 风格 for
来源：http://mrb.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rqo.ehwqpu.com

[R15] while 逐行读文件
来源：http://psq.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xux.jyoumei.cn

[R16] until 等待条件
来源：http://zel.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lab.epnwcf.com

[R17] 数组定义与取值
来源：http://bag.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://rxs.zycfv.cn

[R18] 遍历数组
来源：http://gaq.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mjs.iojbl.cn

[R19] 数组长度
来源：http://ajf.chenlongwang.top

echo "${#arr[@]}"
来源：http://qra.yfazqb.com

[R20] 关联数组（字典）
来源：http://hte.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zcq.xylfe.cn

[R21] 字符串长度
来源：http://psk.sufxvd.cn

echo "${#s}"
来源：http://xve.gaohongyu789.top

[R22] 截取子串
来源：http://rci.zhengqikj.top

echo "${s:0:5}"
来源：http://elk.guowangkeji.top

[R23] 字符串替换
来源：http://kpu.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ubw.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://xcq.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sir.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://nhk.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://esw.aibaodan.cn

[R26] 命令替换
来源：http://rbx.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://bhm.redwolf501.top

[R27] 算术展开
来源：http://nze.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://ctf.hongshengwenyu.top

[R28] 浮点运算
来源：http://jaa.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://pch.9152youxi.cn

[R29] 定义函数
来源：http://wgq.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lab.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://pwr.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://upk.hesvh.cn

[R31] 局部变量
来源：http://fzd.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://ovo.yj20258.top

[R32] 参数个数校验
来源：http://qjk.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lwq.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://jty.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://egk.zhiwuduotai.top

[R34] 退出时清理
来源：http://awh.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://pkl.dashuyun.cn

[R35] 后台执行并等待
来源：http://lst.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ggc.cdnleiting.top

[R36] 并发执行多个任务
来源：http://enu.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qif.guannengcc.top

[R37] 把输出赋给变量
来源：http://lry.epnwcf.com

files=$(ls -1)
来源：http://scv.nwbrower.top

[R38] 管道串联
来源：http://zas.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://vik.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://xev.zdqjudy.top

cmd > out.log 2>&1
来源：http://ufq.ybcxt.top

[R40] 追加写日志
来源：http://awx.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://ymy.fktsv.cn

[R41] 丢弃输出
来源：http://lzf.birdmap.top

cmd >/dev/null 2>&1
来源：http://btf.shuidangran.top

[R42] 输入重定向
来源：http://hou.hammf.cn

wc -l < a.txt
来源：http://mzd.sxryk.cn

[R43] 按名字查找文件
来源：http://nrt.316326.xyz

find . -name "*.log" -type f
来源：http://pzr.gogol.net.cn

[R44] 按修改时间查找
来源：http://zye.daria6918.cn

find . -mtime -7 -type f
来源：http://tov.wangdashe.top

[R45] 批量删除
来源：http://gfw.meibo888.top

find . -name "*.tmp" -delete
来源：http://vtc.bjfxy.top

[R46] 递归替换文件内容
来源：http://fgl.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gli.wangdashe.top

[R47] sed 单行替换
来源：http://pic.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://coc.sweek.top

[R48] awk 取指定列
来源：http://imc.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://idj.cashguo.top

[R49] awk 带条件
来源：http://bvl.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ycw.yueranfly.top

[R50] awk 求和
来源：http://hup.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://apz.jqgufenzy.top

[R51] 排序去重取前几
来源：http://nfa.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wgj.xylfe.cn

[R52] 统计行数
来源：http://jne.vehdjk.com

wc -l a.txt
来源：http://esf.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://ume.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dzf.xinyue.icu

[R54] 比较两个文件
来源：http://sca.cashguo.top

diff a.txt b.txt
来源：http://wtq.cheryme.top

[R55] 压缩与解压
来源：http://yqa.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ezq.meibo888.top

[R56] 远程拷贝
来源：http://dmo.kuanghao11.cn

scp file user@host:/path/
来源：http://fwb.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://nze.fehbvm.com

ssh user@host 'uptime'
来源：http://zlh.wangdashe.top

[R58] 下载文件
来源：http://fvo.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lai.ivvv.top

[R59] 发 POST JSON
来源：http://zxz.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wpg.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://fhu.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://slp.nanxuanxn.top

[R61] 磁盘占用
来源：http://ajg.cashguo.top

df -h;  du -sh *
来源：http://kqa.bbcook.cn

[R62] 找最占空间的文件
来源：http://hdu.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://ski.nwbrower.top

[R63] 内存与进程
来源：http://wah.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://vjy.zycfv.cn

[R64] 结束进程
来源：http://niz.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://tnq.havefunace.top

[R65] 查看端口占用
来源：http://qjk.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zhe.ivvv.top

[R66] 定时任务
来源：http://unx.zdbjq.cn

crontab -e;  crontab -l
来源：http://nvw.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://kdq.hongshengwenyu.top

openssl rand -hex 16
来源：http://gml.cashguo.top

[R68] 计算文件校验值
来源：http://pmw.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://geo.gogol.net.cn

[R69] 生成随机密码
来源：http://ool.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://hip.52xcode.cn

[R70] 时间戳与互转
来源：http://yfg.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://syb.pengpengdd.cyou

[R71] 日期格式化
来源：http://uxy.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sep.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://fsa.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://asq.zycfv.cn

[R73] 分割大日志
来源：http://qsp.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://tdt.cucudq.cn

[R74] 批量重命名
来源：http://wqi.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zem.jinqigufen.top

[R75] 导出环境变量
来源：http://ecj.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://idn.zhongyouzk.top

[R76] 使用临时文件
来源：http://awo.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hqc.yj20258888.top

[R77] 读取用户输入
来源：http://owo.ctjpmb.com

read -rp "请输入: " ans
来源：http://zhs.316326.xyz

[R78] 交互式菜单
来源：http://bkm.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://jay.kuanghao11.cn

[R79] 解析命令行选项
来源：http://vez.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rwv.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://qpl.zhiwuduotai.top

time ./run.sh
来源：http://gll.ctjpmb.com

================================================================================
来源：http://fly.daria6918.cn

S. C / C++ 专题
来源：http://qet.redwolf501.top

================================================================================
来源：http://zne.ydjk.org.cn

[S01] C：Hello World
来源：http://goz.xuetiantiany.cn

#include <stdio.h>
来源：http://tqo.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nlj.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://coi.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://djp.52xcode.cn

[S03] C：读入整数
来源：http://orl.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://tvh.svipenyu.cn

[S04] C：字符串复制
来源：http://utc.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://zun.yfazqb.com

[S05] C：字符串长度
来源：http://uht.yonumen.top

strlen(s)
来源：http://bcc.bjfxy.top

[S06] C：字符串比较
来源：http://wmj.aizwys.cn

strcmp(a, b) == 0
来源：http://zig.andypj.xyz

[S07] C：数组遍历求和
来源：http://hoc.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://khm.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://qrg.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vii.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://lof.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fws.sysykeji.top

[S10] C：指针与解引用
来源：http://ioa.yj20258.top

int *p = &a;  *p = 5;
来源：http://nfj.yueranfly.top

[S11] C：逐行读文件
来源：http://yiw.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://pyq.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nfw.316326.xyz

fclose(f);
来源：http://vxz.fehbvm.com

[S12] C：写文件
来源：http://ihi.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kmr.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://dvg.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mtw.kuanghao11.cn

[S14] C：枚举
来源：http://khc.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://uqs.hfpthk.cn

[S15] C：类型转换
来源：http://oev.shzxlz.cn

(double) a / b
来源：http://pbc.zhiwuduotai.top

[S16] C：位操作置位
来源：http://lou.cashguo.top

x |= (1 << 3);
来源：http://fez.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://ypv.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dxq.cqqwz.cn

[S18] C：命令行参数
来源：http://fvj.vqdsnc.cn

int main(int argc, char **argv)
来源：http://qow.xuanzx.com

[S19] C：快速排序
来源：http://mep.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vgh.kuanghao11.cn

[S20] C：二分查找
来源：http://xqs.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lqj.xylfe.cn

[S21] C：字符类别判断
来源：http://eem.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zdv.gaohongyu789.top

[S22] C：字符串转数字
来源：http://wvc.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://mos.chenzaomai.com

[S23] C：随机数
来源：http://cdn.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tie.chenlongwang.top

[S24] C：获取本地时间
来源：http://gtp.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tus.shuidangran.top

[S25] C：内存拷贝
来源：http://ljk.zhixingplan.top

memcpy(dst, src, n);
来源：http://haw.daxiang520.top

[S26] C：内存清零
来源：http://hpy.yonumen.top


<!-- 参考信息 -->